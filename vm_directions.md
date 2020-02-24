# Using CCAC's virtual Linux machines

### Accessing machines from home through the CCAC VPN:

1. **ONLY the first time you connect!** Go to https://academicvpn.ccac.edu/, and download the appropriate client for your machine. Follow the directions to install it.
1. Open GlobalProtect. If it asks for your portal address, enter **academicvpn.ccac.edu**. Click "Connect."
1. Follow the rest of the directions as if you were accessing the virtual machine from campus.

### Accessing machines from campus: 
1. Go to our VMWare landing page: [https://cit-lab-esxi.ccac.org/ui](https://cit-lab-esxi.ccac.org/ui).
1. Probably you will get a very scary certificate error, and as much as it pains me to tell you this, you need to accept/choose "advanced" and "go ahead" to get through to our virtual machines. Sorry! We know this is bad.
1. Log in with your CCAC credentials.
1. Click "Virtual Machines" in the left sidebar.
1. Click [the virtual machine assigned to you](./week02/vm_assignments.pdf)&mdash;you can only access *your* assigned machine, but you'll be able to see everyone else's.
1. Once you're on your VM's landing page, choose "Console." (If your machine is powered off, you may have to click "Power on" first.) You can choose any of the first three options; I usually go with "Open browser console," because it can be set to full-screen, but you do what you like.
1. The username on the machine appears to be set as "Data Analyst" (it's actually "ccac-data"), and the password is "student123"

Now you are logged into a computer inside your browser window. It has a browser, a terminal, the LibreOffice suite... all the things you'd expect a Linux machine running on your desk to have. This isn't quite the same experience as running Linux on your own machine, but it's the closest we could get you at CCAC, for now, without requiring you all to have a laptop that you dual-boot.

A note: All of our virtual machines are running on a single physical machine, so we will try to be clever with our usage of resources; for instance: perhaps not all running our big QGIS commands simultaneously. :)