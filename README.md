# Virtual Environments
Student: A01688744 - Norma Yoana Pérez Villalva

## Activity
In this activity, you will migrate and solve the package issues regarding a notebook that was created in a `Python 3.7.9` version.

Follow the instructions below to do the activity.
### Run the existing notebook
1. Clone the project `https://github.com/yoanapv/MLOps_Modulo1.git` on your local computer.
2. Create a virtual environment with `Python 3.7.9`
    * Create venv (Windows)
        ```
        py -3.7 -m venv venv
        ```

    * Create venv (mac)
        ```
        python3 -m venv venv
        ```

    * Activate the virtual environment (Windows)

        ```
        venv/scripts/Activate.ps1
        ```

    * Activate the virtual environment (mac)

        ```
        source venv/bin/activate
        ```
        You'll see the name of the virtual environment, in parentheses, at the beginning of the code line.

3. Install libraries
    Run the following command to install the other libraries.

    ```bash
    pip install -r MLOps_Modulo1/requirements_3-7
    ```
    Verify the installation with this command:
    ```bash
    pip freeze
    ```
    Output:
    <details open>
    <summary>List of packages, click to collapse</summary>
  
        appnope==0.1.3
        backcall==0.2.0
        cycler==0.11.0
        debugpy==1.6.7
        decorator==5.1.1
        entrypoints==0.4
        ipykernel==6.16.2
        ipython==7.34.0
        jedi==0.18.2
        joblib==1.0.1
        jupyter-client==7.4.9
        jupyter-core==4.12.0
        kiwisolver==1.4.4
        matplotlib==3.4.0
        matplotlib-inline==0.1.6
        nest-asyncio==1.5.6
        numpy==1.21.6
        packaging==23.1
        pandas==1.3.3
        parso==0.8.3
        pexpect==4.8.0
        pickleshare==0.7.5
        Pillow==9.5.0
        prompt-toolkit==3.0.39
        psutil==5.9.5
        ptyprocess==0.7.0
        Pygments==2.15.1
        pyparsing==3.1.0
        python-dateutil==2.8.2
        pytz==2023.3
        pyzmq==25.1.0
        scikit-learn==0.20.0
        scipy==1.7.3
        seaborn==0.12.2
        six==1.16.0
        tornado==6.2
        traitlets==5.9.0
        typing-extensions==4.7.1
        wcwidth==0.2.6
        
    </details>
    

4. Open the `MLOps_Modulo1/end_to_end_machine_learning_project.ipynb` notebook and click on `Run All`. 
    > **IMPORTANT!**  
    Do not forget to select the Python 3.7.9 kernel you have already created.

    If everything was ok, you should be able to see the last cell with this output:
    ```bash
    Predictions:	 [263527.   331884.02 221119.   ... 105722.   213199.   459125.66]
    ```
**Congrats, the notebook is running in a virtual environment with Python 3.7.9!**

    * Deactivate the virtual environment
        ```
        deactivate
        ```
        You'll no longer see the name of the virtual environment, in parentheses, at the beginning of the code line.


### Migrating to Python 3.10.9
The goal of this activity is to migrate the libraries to a newer version of Python, for this exercise, `3.10.9`.

1. Create a virtual environment with `Python 3.10.9`.
2. Install the `requirements_3-10.txt`
3. Change the notebook to the Python 3.10.9 kernel, and `Run All` cells.  
    If everything was ok, you should see the same output in the last cell as the Python 3.7.9 kernel.

## END