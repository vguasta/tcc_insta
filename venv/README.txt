=======================================================
=======================================================

1 - Install Anaconda
2 - Initialize Anaconda Prompt in this repository as Administrator
NOTE: You can change "envtcc" for any environment name

=======================================================

Change directory to another drive:
	cd /d D:\

=======================================================

See your venvs installed:
	conda info -e

=======================================================

Create a venv by yml in this repository (recomended):
	conda env create -f envtcc.yml -p ./envtcc

=======================================================

Create a new venv in this repository:
	conda create --prefix ./envtcc

=======================================================

Active a venv:
	conda activate <venv_name>
	conda active <venv_path>
	conda activate ./envtcc

=======================================================

Deactive a venv:
	conda deactive

=======================================================

Install pip requirements (not necessary if you loaded a venv by yml):
	pip install -r ./requirements_pip.txt

=======================================================

Export venv infos:
	conda list -e > requirements_conda.txt
	pip freeze > requirements_pip.txt
	conda env export > envtcc.yml
	
=======================================================

Copy venv infos to a backup folder:
	copy requirements_conda.txt .\bkp
	copy requirements_pip.txt .\bkp
	copy envtcc.yml .\bkp
	copy README.txt .\bkp
	
=======================================================

Remove a installed venv:
	conda remove -name <venv_name> --all
	conda remove -prefix <venv_path> --all
	conda remove -prefix ./envtcc --all
	(Restart your computer for a complete clean. If the folder continues existing, you can delete it manually)

=======================================================
=======================================================