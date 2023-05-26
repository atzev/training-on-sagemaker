# SageMaker Labs

**Part 1** 

1. Run the following command in the terminal 

```
git clone https://github.com/aws/amazon-sagemaker-examples.git  
```
2. Navigate to amazon-sagemaker-examples/training/distributed_training/pytorch/data_parallel/mnist/pytorch_smdataparallel_mnist_demo.ipynb

3. Double click on the notebook to open it

4. Navigate to /code/train_pytorch_smdataparallel_mnist.py

Replace lines 259 and 260
```
if args.save_model:
        torch.save(model.state_dict(), "mnist_cnn.pt")
```

with 
```
path = str(os.environ["SM_MODEL_DIR"])
model_path = os.path.join(path, "mnist_cnn.pt")
```
&nbsp; 

**Part 2** 

1. Run the following command in the terminal 

```
git clone https://github.com/aws-samples/sagemaker-distributed-training-workshop.git
```

2. Navigate to sagemaker-distributed-training-workshop/2_model_parallel_sdp/Lab_2.ipynb

4. Double click on the notebook to open it

&nbsp; 


**Part 3** 

1Run the following command in the terminal 
```
https://github.com/aws-neuron/aws-neuron-samples.git
```
2. Navigate to     aws-neuron-samples/torch-neuron/inference/vit /ViT.ipynb

3.  Double click on the notebook to open it

**Step 4:** 
1. Run the following command in the terminal 
```
git clone https://github.com/aws-samples/sagemaker-trainium-examples.git 
```
2. Navigate to sagemaker-trainium-examples/1_text_classification/Fine tune Transformers for building classification models using SageMaker and Trainium.ipynb

3. Double click on the notebook to open it
