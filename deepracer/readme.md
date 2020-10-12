# Introduction

During the 2019 ReInvent, I went through several sessiosn that focused on DeepRacer and Reinforcement ML. The sessions focused on theory and hands-on interaction with DeepRacer.

# AWS DeepRacer

DeepRacer directly relies on several AWS services (S3, Lambdas, Kinesisvideo, CloudFormation, SageMaker, RoboMaker and CloudWatch). To understand how the DeepRacer models are created and tested you have to invest time in the other services. 

I spent several days using the DeepRacer service, it's required services and tested various model changes.

DeepRacer is costly, testing the models needs a lot of CPU. There are around 12 tracks to test your model against. Depending on your approach, if you want a single model to perform well on all 12 tracks, each change to your model will require 12 training sessions. If your requirements are set such that heavy training is needed, the costs can well exceed $1,200 / day.

# Automated Tests via Local Compute

Once I figured out the daily costs to test each model change, I sought out to (1) run the model testing and underlying software to run locally. (2) Automate the testing runs per model change.

Although this was an interesting deep-dive, I was not able to finish the automation. One of the main challenges to these two tasks was hardware. (1) I didn't have enough GPU and memory on my laptop. (2) I needed more diskspace. The model testing (12 tracks) required much more diskspace than what I had available.

# Final

DeepRacer has a lot of underlying services that make up the DeepRacer experience. It was a good exercise to learn the underlying components that make up DeepRacer. I also enjoyed applying Reinforcement ML concepts / techniques through DeepRacer.

It's a great way to introduce a hands-on approach to learning ML for high schools. My biggest concern is the training costs.

If AWS can lower the costs for DeepRacer, I think it would be a great ML education opportunity for high school students (after school).