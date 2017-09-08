# Acquire License
* This is a BYOL (Bring Your Own License) product. Please email support@falcon-computing.com to 
   acquire the license.

# Launch Merlin Compiler Instance
Launch an instance with supported instance types and Merlin Compiler AMI.  
This will set up all environment to run Merlin Compiler.

# Run Merlin Examples
Open a new terminal and run the commands below. Replace access-key and  
instance-IP with your own configurations.
```
$ssh -i <access-key> centos@<intacne-IP>
$cd merlin-examples/vec_add/build
$make run
$make mcc_acc
```
Merlin Compiler will optimzed application code in vec_add_kernel.mco.

