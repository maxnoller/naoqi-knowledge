# naoqi-knowledge
I AM NOT AFFILIATED WITH ALDEBARAN IN ANY WAY. ANY COPYRIGHT OR LICENSES REGARDING NAO, ALDEBARAN, NAOQI, QI and PEPPER BELONG TO THEM.
If this somehow is not ok license/copyright wise please message me I will take it down immediately.

This repository is supposed to be a collection of knowledge I build over the years working with Aldebaran robots in python. The official documentation is very confusing and I've spent countless hours of my life figuring things out that I wont get back so I thought I would write some down here to hopefully save someone else some time/sanity.

## Questions/suggestions/corrections
If you have any questions regarding working with the robots in python, suggestions or wishes on how to expand this repo or corrections for mistakes in this repository please create an issue.

## SDKs
### QI or NaoQI? Can I use python 3 to work with Aldebaran robots?
A lot of sources on the Internet claim you need to use python2.7 to work with Nao and while this might have been true in the past, at some point Aldebaran has blessed us with an updated SDK for python.
#### NaoQI
This is the older sdk used in most of the tutorials/resources online. It requires python 2.7 and cannot be installed from pip as far as I am aware. You should not use this anymore, I dont think they are still updating it, python2.7 is ancient and should not be used under any circumstances and it is in general just a pain to work with.
#### QI
Newer SDK which supports python3, is still being updated (sometimes) and is just in general a way better experience to work with.
You can install QI using pip (or similar package managers like poetry): `pip install qi`

