# Gandalf
Gamma Spectra Identification

I have added a word document that secribes the goal and Path of the project

I am adding word documant as a bin file and I am copying test below:

Spectrum Project	November 26, 2019 Dr. Kenneth B Butterfield

The goal of the spectrum project is to identify isotopes and sums of isotopes from gamma spectra with varying amounts of shielding using machine leaning. 

I will use deep learning based on neural nets. 
The nets will need to use softmax output layers and there will be two layers. One for single outputs and one for sum of outputs. With third binary layer that signals which output to report.
The cost function will be the surprise cost function to promote fast learning.
The project will start by using tuples of energy and area to define an isotope and PeakEasy peaks and areas as inputs. Alternatively; tables from the spectraDeck could supply the data.
I can enlarge the training set by using monte carlo to grow the observed spectra and then use Peak easy to find tuples. Will it work in batch mode? Does Scott have tools that would work in batch mode.

A proof of concept experiment would be to use the network programs in the ‘deep learning’ book that identify numerals and extend by mixing numerals in a single input. Add softmax layers for the outputs. Train with singles but build test library of summed numerals.

If we extend to shielding we need peaks and areas and relative size of associated Compton downscatter. Does PeakEasy return this type of parameter? Does Scott have a gamma generator similar to Neutron Generator? Gadras is Sandia generator. Are there rules to relate this ratio? Could a neural net be trained to find peaks, downscatter, areas, and ratio? 
Scott thinks that starting with the spectra direction may be the best idea. Let it figure out Compton and must have rules. We could use Gadras to generate shielded spectra and determine type of shielding. While I had thought of this option Scott has convinced me that this is a good way to go.
If one doesn’t exist, a montecarlo simulation could change resolution, downscatter in external shielding, (slab box shell), account for detector material and size through Eff(energy) with potential compton loss in detector. Ie slowing down distance and escapes through side of scattered rays. This could be a project on its own. I hope Gadras might suffice for now.

Path
The Neural Networks and Deep Learning book by Michael Nielsen is my main reference. 
It uses Python as the language.
Programs from book implement the network and learning algorithms.
First experiments will be to get character recognition working. 
Second is to get single spectra working
Third is to add layers to get sums of characters and character counting working.
Fourth is to get sums of spectra and counter working
Github has the code and documents. I can use this for project management, version control, and to allow peer interaction or review. I am signed up and will put this document into the README file of the Spectra project.
Scott has agreed to be peer. Rooney has not got back with me. Steve might be another person to get involved.

Steve Myers has gamma spectra and we could convolve to get NaI data.



