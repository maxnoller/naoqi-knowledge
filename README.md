# NaoQI Knowledge

**Disclaimer:** I am not affiliated with Aldebaran in any way. Any copyrights or licenses regarding NAO, Aldebaran, NAOqi, QI, and Pepper belong to them. If there are any issues regarding licenses or copyrights, please message me, and I will take it down immediately.

This repository is a collection of knowledge I have built over the years working with Aldebaran robots in Python. The official documentation can be very confusing, and I've spent countless hours figuring things out. I hope this repository saves someone else some time and sanity.

## Questions, Suggestions, and Corrections

If you have any questions about working with the robots in Python, suggestions for expanding this repo, or corrections for mistakes, please create an issue.

## SDKs

### QI or NaoQI? Can I use Python 3 to work with Aldebaran robots?

A lot of sources on the internet claim you need to use Python 2.7 to work with NAO. While this might have been true in the past, Aldebaran has updated the SDK for Python.

- **NaoQI**  
  This is the older SDK used in most tutorials and resources online. It requires Python 2.7 and cannot be installed from pip. It is outdated and should not be used, as Python 2.7 is deprecated.

- **QI**  
  This is the newer SDK, supporting Python 3 and still being updated occasionally. It provides a better experience overall.
  
  **IMPORTANT:** The PyPI version is only available for Linux. Aldebaran does not provide a Windows version of QI. To use QI on Windows, use [WSL](https://learn.microsoft.com/en-us/windows/wsl/install). 

  You might be able to compile QI for Windows yourself. If I attempt this, I will post a guide here. If anyone else manages to do this, please let me know.  
  You can install QI using pip (or similar package managers like Poetry): `pip install qi`

---
