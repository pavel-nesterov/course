In this video, I'm going to give you a very quick introduction to how our transformers models work together with Tensorflow and Keras! The very short explanation is that all of our Tensorflow models are also Keras model objects, and so they have the standard Keras model API. If you're an experienced ML engineer who's used Keras a lot, that's probably all you need to know to start working with them. But for everyone else, including the prodigal PyTorch engineers out there who are returning to the fold, I'm going to quickly introduce Keras models, and how we work with them. In other videos, which I'll link below, I'll run through training with Keras models in more detail. But first, what is a Keras model? Your model basically contains your entire network: It contains the layers, and the weights for those layers, and also tells the model what to do with them; it defines the whole path all the way from your inputs to your outputs. If you've used Keras before, you probably started by building your model out by hand - you added one layer after another, maybe using model.add() or the functional approach. And there's nothing wrong with that! But you can also pre-load an entire model, weights and all. This is really helpful, because if you try reading the paper or looking at the code, you'll see the inside of a Transformer is pretty complex, and writing it all out from scratch and getting it right would be hard even for an experienced machine learning engineer. But because it's all packed inside a Model, you don't need to worry about that complexity if you don't want to! You have the flexibility to write any model you like, but you can also just load a pre-trained, pre-configured transformer model in one line of code. And whether you write your own model from scratch or load a pre-trained one, you interact with the model in the same way - through the same few methods you're going to see again and again, like *fit*, *compile* and *predict,* and we'll cover concrete examples of how to use those methods in other videos that I'll link below. For now the key thing to take away from this video, if you've never seen Keras before, is that this neat encapsulation means that all of the complexity of a huge neural net becomes manageable, because you interact with it in exactly the same way, using exactly the same methods, as you would with a simple model that you wrote out by hand.