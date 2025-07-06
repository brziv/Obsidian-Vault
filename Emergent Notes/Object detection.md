#application 

SIC 2025 project.

I start doing the project after dealing with the beast named System 1.
	I declare a mental check procedure as a weapon in my armory.

Collect the dataset from Kaggle:
	Analyze total class distribution and across splits (images and boxes)
	Bounding boxes per image distribution (log scale)

Preprocessing:
	I notice that the splits are not stratified (class with 0 image)
	Merge splits, filter images with >20 boxes, stratified split

Training:
	YOLOv8s, optimizer `SGD`, augment, cache `disk`
	Freeze 10 layers first 20 epochs, then unfreeze for the rest

Next:
	Quantization, pruning
	Test-Time Augmentation
	Class 0: class weighting, focal loss
		Going to find a solution for this