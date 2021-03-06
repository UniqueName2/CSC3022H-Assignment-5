**CSC3022H-Assignment-5

**C++ Simple Audio Manipulation Program (samp)

Author : Sahil Patel

Student Number : PTLSAH004

Date : 05-June-2017

***Usage: Please have the neccessary files in the same directory when running.

*'$' refers to the command line

To compile - 
	$make

To Run - 
	$samp -r sampleRateInHz -b bitCount -c noChannels [-o outFileName ] [<ops>] soundFile1 [soundFile2]
	
	Description:
		•-r Specifies the number of samples per second of the audio file(s) (usually 44100)
		
		• -b Specifies the size (in bits) of each sample. Only 8bit and 16bit should be
		supported in your program. More on this later on.
		
		• -c Number of channels in the audio file(s). Your program will only support 1 (mono) or
		2 (stereo).
		
		• “outFileName” is the name of the newly created sound clip (should default to “out”).
		
		• <ops> is ONE of the following:
		
			• -add: add soundFile1 and soundFile2
		
			• -cut r1 r2: remove samples over range [r1,r2] (inclusive) (assumes one sound
			file)
		
			• -radd r1 r2 s1 s2 : add soundFile1 and soundFile2 over sub-ranges indicated
			(in seconds). The ranges must be equal in length.
			
			• -cat: concatenate soundFile1 and soundFile2
			
			• -v r1 r2: volume factor for left/right audio (def=1.0/1.0) (assumes one sound
			file)
			
			• -rev: reverse sound file (assumes one sound file only)
			
			• -rms: Prints out the RMS of the sound file (assumes one sound file only).
			More details will be given later on.
			
			• -norm r1 r2: normalize file for left/right audio (assumes one sound file only
			and that r1 and r2 are floating point RMS values)
			
			
		• “soundFile1” is the name of the input .raw file. A second sound file is required for
		some operations as indicted above. 

To test -
	$make tests
	
Please refer to the document Tutorial_5.pdf for more details regarding this assignment.

Please feel free to contact me at sahil.j.patel@gmail.com should you require any further clarification. Thank you.
