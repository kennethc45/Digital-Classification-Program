# Project 1: Digit Classification

In this project you will implement a naive Bayesian classifier for a set of scanned handwritten digit images. Your task is to guess which digit a handwritten image is supposed to be. To help, you are given a set, or corpus, of training images which have already been labeled with the correct digits. The goal of a classifier is to compute the most likely digit for an unclassified image, by breaking the image apart into features and ranking each digit by how closely it matches the image.

The detailed description for this project can be found on the [course webpage](https://sites.google.com/trinity.edu/csci2322-fl22/individual-projects/project-1-digit-classification).

## Timeline
* Friday 8/26 - Project Released
* Wednesday 8/4 - Milestone One deadline
* Tuesday 9/6 - Milestone Two deadline
* Monday 9/12 - Project submission deadline. 
* Wednesday 9/14 - Late submission deadline. 



Student Name:
Trinity ID: 

Core Project: 75/75
Implementation: 4/8
Smoothing: 7/7
Avoiding Work: 0/10
Project 1 Grade: 86/100 (B+)

Project Check: grep "type Corpus" DigitRecognition.hs
type Corpus = [(Digit, [PixelImage])]

Project Evaluation: --forceTests --quiet
required code style: passed 
Failed for any error when more than 1 match: 
			Did not return an exception
Failed for a non-Prelude error when more than 1 match: 
			Did not return an exception
Failed for a non-Prelude error when 0 the key is missing: 
			Failed, returning the built-in exception: Prelude.head: empty list
lookupVal implementation details: failed with 0/4
Failed that you've updated Corpus definition: 
			Corpus should not be type Corpus = [(Digit, [PixelImage])]
Failed that your code is linear in the number of training images: 
			Failed! Your solution is probably linear or n*log(n). 
			Increasing input size from 128 to 256 increased the runtime from 0.938s to 1.629s, a factor of 1.736
that you avoid unnecessary work: failed with 0/10
full credit: failed with 11/25
Failed that you do not use nested list comprehensions: 
			should not use nested list comprehensions
			Nested list comprehension in: [(x, [fst img | img <- imgLbls, snd img == x]) | x <- nub [snd img | img <- imgLbls]]
common style mistakes (optional): passed 
Failed detect maximum rank of 0 on 55th image: 
			Failed, returning the built-in exception: Prelude.head: empty list
classifyImage implementation details (optional): passed 
optional requirements: passed 
Project 1: failed with 86/100
TIME: 4.348
Project 1: failed with 86/100

