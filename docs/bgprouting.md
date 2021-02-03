## **Network Parser Demo**


two different methods to deploy the same BGP configuration.
- template based 
  - using JINJA templating engine
  - config module
- resource module based

both methods using the same data structure here
inventory definition:
https://github.com/maxrainer/network-demos-inventory/tree/nxos

## **Demo Workflow**
- clear BGP config from device 
- explain inventory and BGP host variables 
  - show in IDE first 
  - show on inventory on tower
- template bases config
  - run BGP ROUTING 0001 - template based config 
  - run a second time to show idempotency
  - show bgp template on IDE
  - change inventory on tower
    - add a vrf to config 
```
    - neighbors:
        - neighbor_address: 10.10.10.10
          remote_as: '11111'
      vrf: vrf3
```
- resource module configuration
  - run with same inventory ==> no changes done
  - explain state "replaced" - "merged" 
  - explain "before" and "after" in playbook output
  - clear bgp config from device
  - run again
  - goto playbook output, explain commands etc...
- run NET PARSER 0001 - general parser
  - limit to nx9k
  - "show bgp sessions"
  - pyats parser