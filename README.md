# Data analysis
- Document here the project: fooproject
- Description: Project Description
- Data Source:
- Type of analysis:

Please document the project the better you can.

# Startup the project

The initial setup.

Create virtualenv and install the project:
```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
make clean install test
```

Check for fooproject in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/fooproject`
- Then populate it:

```bash
##   e.g. if group is "{group}" and project_name is "fooproject"
git remote add origin git@github.com:{group}/fooproject.git
git push -u origin master
git push -u origin --tags
```

Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
fooproject-run
```

# Install

Go to `https://github.com/{group}/fooproject` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:

```bash
sudo apt-get install virtualenv python-pip python-dev
deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:

```bash
git clone git@github.com:{group}/fooproject.git
cd fooproject
pip install -r requirements.txt
make clean install test                # install and test
```
Functionnal test with a script:

```bash
cd
mkdir tmp
cd tmp
fooproject-run
```
