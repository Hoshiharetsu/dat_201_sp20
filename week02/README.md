# Week 2

## Agenda
0. [Announcements](#announcements)
1. [Talking about the readings](#readings)
2. [Showing off what we found with grade data](#grades)
3. [Getting into Linux](#vmware)
4. [Linux intro](#linux)
5. [Install QGIS](#installation)
6. [Homework](#homework)

## <span id="announcements">0. Announcements</span>

I think [this looks like a really good addition to our course](https://pitt.libcal.com/calendar/today/pghhistories). Unfortunately for most of us, it's in Oakland in the middle of the day. Can anyone make it? If not, I might try asking _really nicely_ to see if these folks can come talk to us. 

## <span id="readings">1. Talking about the readings</span>

Thoughts? Reactions? Was any of it surprising? Which parts of this seemed good and reasonable, which parts seemed like overstepping, and where do we think the line is? Would the line be in a different place if we were talking about employees instead of students? 

## <span id="grades">2. Showing off what we found with grade data</span>

Hopefully everyone's spreadsheets are in the [shared folder](https://acdccac-my.sharepoint.com/personal/edarsow_acd_ccac_edu/_layouts/15/onedrive.aspx?e=5%3A0721e98802b54c18b12d59ea6e9a9dc2&at=9&CT=1580172664342&OR=OWA%2DNT&CID=fac0b577%2D44b5%2D1d03%2D2c90%2D9cc34d7ca0ee&FolderCTID=0x0120003C700CE6FEE4A548B6EB8A40653D4910&id=%2Fpersonal%2Fedarsow%5Facd%5Fccac%5Fedu%2FDocuments%2Fdata%5Fanalytics%2Fdat%5F201%5F20sp%5Fstudent%5Fwork%2Fdata%5Fcleaning%2Fgrade%5Fcomparisons), so they can be pulled up on the big screen. I'll emcee the discussion, but I want you to have the chance to show off your findings to one another . 

## <span id="vmware">3. Getting into Linux</span>

I'm going to give you the steps you'll follow to access these machines from home, but **you can skip the first two while we're on campus**:
1) We need to connect to the CCAC VPN. Go to [https://academicvpn.ccac.edu/](https://academicvpn.ccac.edu/), and download the appropriate client for your machine.
2) Install it, and when it (a piece of software called GlobalProtect) opens, it will ask for a portal address. Your portal address is academicvpn.ccac.edu. 
3) Next, we need to go to our VMWare landing page: [https://cit-lab-esxi.ccac.org/ui](https://cit-lab-esxi.ccac.org/ui).
4) If you're off campus, you'll get a very scary certificate error, and as much as it pains me to tell you this, you need to accept/choose "advanced" and "go ahead" to get through to our virtual machines. Sorry! On-campus, it should just work.
5) Log in with your CCAC credentials.
6) Click the virtual machine assigned to you, which you can look up in [the PDF in this directory](./vm_assignments.pdf) --you can only access your assigned machine, but you'll be able to see everyone else's. 
7) Once you're on your VM's landing page, choose "Console." You can choose any of the first three options; I usually go with "Open console in new tab," but you do what you like.
8) The username on the machine appears to be set as "Data Analyst" (it's actually "ccac-data"), and the password is "student123"

Now you are logged into a computer inside your browser window. It has a browser, a terminal, the LibreOffice suite... all the things you'd expect a Linux machine running on your desk to have. This isn't quite the same experience as running Linux on your own machine, but it's the closest we could get you at CCAC, for now, without requiring you all to have a laptop that you dual-boot.

A note: All of our virtual machines are running on a single physical machine, so we will try to be clever with our usage of resources; for instance: perhaps not all running our big QGIS commands simultaneously. :) 

## <span id="linux">4. Getting to know and love Linux</span>

### A short todo list, especially for people who are new to Linux:
* Open LibreOffice Writer. (Bonus: find a second way to open it.)
* Find and open the web browser. Navigate to some website you like.
* Use File Manager to figure out the layout of your system. Make a little map for yourself. (You can hand-write it. Or, consider typing the map either in LibreOffice Writer on the virtual machine, with occasional backups to somewhere else, or else in Word/Writer/Pages on your local machine, with backups to a USB drive or the cloud. I'm going to ask you to start keeping notes with useful Linux commands, anyway.)

As you've seen, you have a graphical user interface on this machine. You can fall back on that when you need to (and, you know, the whole time we're using QGIS), and most of it will work a lot like Windows and Mac. (More like the former than the latter, in my opinion, which is funny, given that the inner workings of a Mac are more like the inner workings of Linux.) But the real power is in using a command line interface, which I'd like to show you&mdash;some of you for the second time. :) 

### Things I want to cover about CLIs with you:
* Pieces of a command prompt.
* Why we don't put spaces in filenames.
* Directory structures if we somehow blew past that during the "make a map of the machine" phase of the evening.
    * Absolute versus relative paths.
* Previous command shortcut.
* Tab completion.

And, you know, everything on the [cheat sheet](./cli_cheat_sheet.md).

## <span id="#installation">5. Now let's get QGIS on this machine</span>

We're going to [install QGIS](https://qgis.org/en/site/forusers/alldownloads.html#linux)

Some notes: they give us directions, but we're going to need to think about them a bit to determine how best to follow them. For sure, we need to figure out which version of Linux we're running (`uname -a`) and to decide which version we want (Long-Term Release). 

## <span id="homework">6. Homework for this week</span>

### Linux practice:

We need to get comfortable with Linux. Check out a book, work through some tutorials, install some software you think you'll find useful, try and break your system&mdash;whatever it is you need to do to get comfortable working with Linux and especially on the command line. (Track the time you spend on this, please.) 

If you somehow do successfully break your system, first off: it happens, no biggie; document what went wrong. Maybe we can fix it. Secondly: I can issue you a new one, with some help from ITS, but it won't be immediate, so let me know as soon as you can.

### Readings - come prepared to discuss:
* Wiseman, Andrew. "When Maps Lie." CityLab. 06/25/2015. [link](https://www.citylab.com/design/2015/06/when-maps-lie/396761/)
* Rannard, Georgina. "Australia fires: Misleading maps and pictures go viral." BBC News. 01/07/2020. [link](https://www.bbc.com/news/blogs-trending-51020564)