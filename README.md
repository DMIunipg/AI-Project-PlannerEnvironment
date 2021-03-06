AI-Project-PlannerEnvironment
=============================

An environment to test a planner agent, created for a college project and based on a problem from "Artificial Intelligence: A Modern Approach" by Stuart Russell and Peter Norvig.

## Dependencies

All you need is python. This module is tested on python 2.7.5 and 3.3.2.

## Run the application

You can create your Agent in the *agents_dir*, like MyAgent example. The name of the file must be the same
of the class that you create. The class must *inherit from LogAgent* and you have to implement the
method *solve*.

You can put your configuration file in *cfg_dir*. These files must be with json extension and they must respect
the sintax of the environment, like in the examples that you can see in this directory.

To run the application simply execute the main.py file:

```bash
python main.py [-c cfg_list] [-a agents_list]
```

**NOTE**:
* cfg_list is a list of configuration files names.
* agents_list is a list of agents names.  

*Example*: 
```bash
python main.py -c testconfig_simple.json testconfig.json -a MyAgent
```

##Generating random maps

This module comes with a handy random map generator. The sysntax to use it is as follows:
```bash
python cfg_generator.py config_file_name num_airports num_airplanes num_boxes min_num_of_goals
```
This command will create a `config_file_name.json` file under `\cfg_dir`. There is no need to 
add .json at the end of the file name.

Please note that `cfg_generator.py` will always overwrite files with the same name you enter.

## Contributing

Contributions are welcome, so please feel free to fix bugs, improve things, provide documentation. 
For anything submit a personal message or fork the project to make a pull request and so on... thanks!

## Notes

This library is under heavily development, so there may be substantial changes in the near future.  

You can find an example of utilization of the module in this repo. Detailed instruction will be written soon.

## License

[The MIT License (MIT)](https://raw.githubusercontent.com/DMIunipg/AI-Project-PlannerEnvironment/master/LICENSE)
