In order to get the HComb libraries working I have a file (also found here called morph.sh) in my $CERN_BOX home with the following line in it:

source /cvmfs/atlas.cern.ch/repo/ATLASLocalRootBase/x86_64/root/6.04.16-HiggsComb-x86_64-slc6-gcc49-opt/bin/thisroot.sh

This is excecuted under the option for Environment variables in SWAN. Then you can run all these examples yourself in SWAN. No other setup required.


Issues:

1) TCanvas: I'm still in contact with the SWAN developers about using the ugly rootnotes libraries. This is an old hack for displaying TCanvases inline when using notebooks. SWAN needs ROOT:6.07 and the HComb ROOT release is still stuck on 6.04. Is there any plans to include these libraries in the current root dev plan? otherwise we might ask to build ATLASLocalRootBase against a more recent version of ROOT, ideally every night against the dev3 slot.

2) C++: I tried porting example one over to a ROOT C++ notebook. The SWAN guys say that since ROOT 6.04 is not notebook compatible it's very unlikely that we can get C++ examples in this same format until you upgrade

3) Exercise 7 - Working with workspaces: Excercise is bugged when opening and closing the workspace. Error follows. Plots are still made but since the pointers are being set to 0, both the morphing and the fit do not nearly match the validation:

4) General: All tutorials are very bland and 'codey'. More physics and description/explaination would be nice. This is written in markdown so it's easy to make it pretty. I added in a few basic background things and whatever I could find on the twiki page you keep linking to in Lesson 1 such that everything is together. There's a cheatsheet for markdown below:

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

Last edited 24.03.16 by Vince