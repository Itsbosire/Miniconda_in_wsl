# Accessing windows files via wsl
```
cd /mnt/c/Users/HP/
```
Then you navigate to the directory of your choice.
i.e :
```
cd  /mnt/c/Users/Hp/Downloads/
```



# Miniconda in Windows
## Steps in downloading Miniconda
## Install
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

## Install it
```
bash Miniconda3-latest-Linux-x86_64.sh
```

## After Installation
To install conda's shell functions, first restart your shell, then
```
conda init
```

If you'd prefer that your conda' base environment is not activated on startup, set the auto_activate_base parameter to false:
```
conda config --set auto_activate_base false
``` 
## Remove the installation file from your directory
``` 
rm Miniconda3-latest-Linux-x86_64.sh
```

### Using Miniconda
To get into your conda env
```
conda activate
```

### Creating a new environment
```
conda create --name <Env_name>
```

- conda create --name bioinfo_env

### Listing all your environments
```
conda env list
```
# Second session installing Samtools via conda
- Create a new environment
```
conda create --name bioinformatics
```

 Activate the newly created environment
```
conda activate bioinformatics
```

Once the environment has been activated install the tool

```
conda install -c bioconda samtools
```
