# Create repository with command 

Allows you to create a new repository from the linux terminal, it automatically uploads the readme to the created repo leaving it ready to work on


How to configure

```bash 
git clone https://github.com/4ions/Create_auto_repo.git

cd Create_auto_repo
```

the file with the name "new_repo" has to be changed to the address in which the repository was cloned

```bash
python /your/path/where/do/the/clone/create_repo.py --name $1
```

example:

```bash
python /home/Create_auto_repo/create_repo.py --name $1
```

move the file named "new_repo" to the /bin location

```bash
mv new_repo /bin/
```

modify the file named info.py with the user data, path and github token, as shown below 

```python
path = "your/path/where/repo/will/be/created"
user = 'USERNAME'
GITHUB_TOKEN = "YourAcessToken"
```

It is necessary to install with [pip](https://pip.pypa.io/en/stable/) the requirements.txt file

```bash
pip install -r requirements.txt
```
## Usage

Now, with the command new_repo, we can create a new repository as shown in the example below

```bash
new_repo test
```

this will create a new repository with the name test, you can also create a private repository with the flag --private

```bash
new_repo test --private
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
