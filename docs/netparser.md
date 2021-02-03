
## **Network Parser Demo**

### **further links**

### **included roles**
[network_reporting ](https://galaxy.ansible.com/maxrainer/network_reporting)

## **Demo Workflow**
-  start NET PARSER - general parser
   -  talk about different parsers
   -  show pyats parsers parsers https://developer.cisco.com/docs/genie-docs/
   -  talk about ntc_templates and textfsm
   -  show source code of templates in visual studio
- start NET PARSER 0003 - generate JSON inventory 
  - JSON output
  - open in secure CRT
  - show p.e. http://172.16.1.9:81/nx7k-1_inventory.json
- start NET PARSER 0002 - generate HTML reports 
  - show jinja template of HTML side
  - result: http://172.16.1.9:81
- start NET PARSER 0004 - gather facts
  - second way to parse data
  - pre defined commands and parser
  - replaces build in Ansible fact collecting
  - select fact subset
  - select network resource ==> input for resource modules

