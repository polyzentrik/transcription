# Open-source transcription resources
Down-to-earth transcription resources for low-frequency tasks.

## Intro
This repo contains transcription scripts under an Apache 2.0 [license](LICENSE-2.0.txt).

## Objective
The idea is to provide a freely accessible resource to people and organisations that need sustainability transcriptions sporadically. 

As such, the scripts are *designed to run on relatively humble personal computers*. 

They have been tested on a good (CORE i7, 16MB RAM) but still affordable (€500) computer. Waiting times are significant, up to 3 or 4 times the audio length for the most complex script. However, the quality of the results is very satisfactory – comparable to most commercial alternatives available.

For obvious reasons, thus, the scripts are **NOT** meant for production or high-frequency usage.

## Scripts
There are currently three scripts available.

### Simple
This script performs a simple transcription. Audio is transcribed into a TXT file with many lines.

### w. Segmentation
This script adds speaker segmentation to the results of the simple model. It detects when there are speaker changes and then matches Whisper’s transcription to these timings. The output is a TXT file split into paragraphs roughly based on speaker changes (and pauses).

### w. Diarisation
This script takes a more sophisticated approach to speaker diarisation. It detects and labels speakers, breaks the main audio file into smaller audio segments corresponding to each speaker, transcribes each audio segment, and finally joins everything into a single TXT file split into sections labelled by speaker.

## Instructions
Pending.

## Examples
The examples folder contains examples of transcriptions performed with the scripts in this repo.

## Prompts
The diarisation script allows usage of an external prompt file, which can increase the quality of the output. The prompts folder contains examples of prompt files applicable to sustainability.