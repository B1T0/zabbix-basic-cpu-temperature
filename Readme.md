# Zabbix Basic CPU Temperature
This is a very basic template for Zabbix to monitor CPU temperature of Linux machines based on [this](https://myopsblog.wordpress.com/2016/06/06/cpu-temperature-monitoring-with-zabbix/) blogpost.


## How to Install

### Configure Zabbix Agent
1. Make sure lm-sensors is installed. If not use `sudo apt install lm-sensors` to install it.
2. Copy userparameter_cputemp.conf to /etc/zabbix/zabbix_agentd.d/.
3. Restart zabbix-agent using `sudo systemctrl restart zabbix-agent`.

### Configure Zabbix web-panel
1. In Configuration>Templates click on Import.
2. Choose Template basicCPUTemp.xml and click on Import.
3. Check whether temperature data is sent to Zabbix web-panel in Monitoring>Latest Data.
4. Create Screens and monitor your servers!

## What to do in case of errors
NEW: Sadly I am not actively using this little piece of software any longer. Please feel free to [create issues](https://github.com/B1T0/zabbix-basic-cpu-temperature/issues/new) and pull requests. I will review them from time to time.
- Also check [the blogpost](https://myopsblog.wordpress.com/2016/06/06/cpu-temperature-monitoring-with-zabbix/) this template is based on to get to know how this works.
