
                       Sound Creation Laboratory - Lab4
                       ................................



Team Members : Albin Andrew Correya (U127113)
	       Javi Arredondo Garrido (U126744)



Synthesis DTMF tones and personal project sounds in Pure-Data
 


Task 3 
Sub-patch


The pd sub-patch "tline~.pd" is basically used as a filter to reproduce our output signal to 
sound like in a telephone, since the frequency range (bandwidth) of signals is more or less 
between 250 and 3000 Hz. In the sub-patch we use two band-pass filters ("bp~") and two high-pass
filters ("hip") to get our desired effect.

You can find the patch in the folder.



Task 4 
Dial Tones

* Tone 1 : It's the sound of a phone ring that we usually used to hear. It's synthesized 
  by combining sine waves of frequency 480Hz,440 Hz and also bandpass filtered signal fed 
  from the metro object to imitate the ringing sensation of sound.


* Tone 2 : It's a typical DTMF tone inorder to convey that the phone we are calling is out 
  of order.It's synthesized from two sine waves of frequencies 350Hz & 450Hz respectively. 
  Later it's fed to "tline" sub-patch to clip and filter the signal to create the 
  sensation of hearing it in the speakers of telephone.


* Tone 3 : It's a typical DTMF tone to convey us the message that the person we are calling
  is busy with another call. It's synthesized by adding two sine waves of frequencies 
  480Hz and 620Hz then multiplying with a low-pass filtered signal inorder to break the 
  output in regular intervals to create the desired sound.


We have recorded the sound of phone ringing using the "writesf~" object in puredata. 
You can find audio file named "ringing.wav" along with this file.



Task 5 : Synthesized sounds for the final project

Chromones - "The story of Universe"

Our final performance is based on telling the story of origin of universe through soundscapes.
Since most of the sounds in our soundscape are more creative rather than emulating real sounds,
we often used synthesis of electronic sounds to convey our story. 

In this task we are sharing one of the patches we make to emulate the sounds of lava,
chemical bubbles & reactions etc that involves in the creation evolution of earth.
Since we want to control and express various characteristics of sound in real-time while our
live performance, we created a PD patch that could adapt to create these various kind of sounds
having some similar properties. Moreover we are trying to accomplish with a procedural-audio 
synthesis approach.

Check the PD file "Synth_Chemicals.PD" along with this file. Also attached some sample audio of
the patch (with real-time changes in parameters).


* About the patch :


The main components in our patch is nothing but two basic LFO's (Low frequency  oscillators)
and a FM synthesis module. Main idea is to multiply the signals of one LFO along with carrier frequency
signal and other one with modulation index of FM module respectively. Low frequency oscillator
fed into the signal line with carrier signal will create a bubble like audio and the LFO fed into
the modulation index provides us the character and harshness of the sounds that we seek in various
moments of the soundscapes. We can create various kind of sounds by changing the parameters in LFO.You can select different waveforms such as sine,square,sawtooth and noise inside LFO.
We also used the "freeverb~" object and our own delayline patch named "echo-delay" to more or less
emulate the reverberation of open space. Finally it's fed to the output module.Beside that we also
recorded some sound samples from the patch using the "writesf~" object in PD. You can also find it along 
with this.

More details can be found on the PD patch !



Some Future additions to our Pure-Data patch : 

* Synthesizing more different kind of sounds and PD patches needed for the project.

* Map our smartphones and tablets to send and receive OSC messages in from and to our 
  puredata patch inorder to expressively control various parameters of sound in realtime.

* Using machine learning techniques with gestures inorder to interact with the synthesizer 
  in real-time.






<<<<<<.........................................>>>>>>>


