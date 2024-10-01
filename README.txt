# easyUVM
A simple UVM example with DPI 
You can find an explanation of the UVM testbench of the adder module on  https://sistenix.com/basic_uvm.html

Some Learning Notes taken

Each class has simulation phases that are ordered execution steps implemented as methods. The most important UVM phases are:

    the build_phase is responsible for the creation and configuration of the testbench structure constructing the components of the hierarchy
    the connect_phase is used to connect different sub components in a class
    the run_phase is the main phase, where the simulation is executed
    the report_phase can be used to display results from the simulation 

To implement some important methods in classes and variables, UVM provides the UVM Macros. The most common UVM macros are:

    uvm_component_utils: registers a new class type when the class derives from the class uvm_component
    uvm_object_utils: similar to uvm_component_utils, but the class is derived from the class uvm_object
    uvm_field_int: registers a variable in the UVM factory. This macro provides functions like copy(), compare() and print()
    uvm_info: prints messages during simulation time in the environment
    uvm_error: this macro sends messages with error logs 


Virtual method
- Use virtual method whenever you can

DPI vs VPI
- I think both can do similar thing.
