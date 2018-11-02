Packer_ubuntu
# Building our Vagrant Image
Let’s create our image. Run the following command from the directory our JSON file is located.
```cmd
    packer build ubuntu1804.json
```
Adding Our New Box to Vagrant

Our box is built and ready for use. The final step needed is to add the box to Vagrant. Most boxes are pulled down from the Internet, but we need to add a local box. The following command will add your new box to Vagrant.
```cmd
vagrant box add ubuntu1804-vagrant.box
```

To use it in your Vagrantfile, use the name you specified in the builder’s section. In our example, we called our box ubuntu1804-vagrant. The following is an example Vagrantfile that uses our new box.