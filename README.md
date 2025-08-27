Paste the follwoing commands in TCL console in VIVADO to run simulation

1) set_property -name {xsim.simulate.xsim.more_options} -value {} -objects [get_filesets sim_1]
2) set_property -name {xsim.elaborate.more_options} -value {-uvm_testname my_case0} -objects [get_filesets sim_1]
3) run -all

In place of my_case0-

1) To run the simultaneous read/write test: 
+UVM_TESTNAME=my_case0 


2) To run the stress test: 
+UVM_TESTNAME=my_case1 


3) To run the write-full/read-empty test: 
+UVM_TESTNAME=my_case2 

