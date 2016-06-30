PROJECT_ROOT=/home/eyesis/git/oc_jpegencode
TOPLEVEL=jpeg_top
MODULE = test_jpeg_top
VERILOG_SOURCES = $(PROJECT_ROOT)/code/jpeg_top.v  \
 $(PROJECT_ROOT)/code/fifo_out.v  \
 $(PROJECT_ROOT)/code/ff_checker.v  \
 $(PROJECT_ROOT)/code/sync_fifo_32.v  \
 $(PROJECT_ROOT)/code/pre_fifo.v  \
 $(PROJECT_ROOT)/code/sync_fifo_ff.v  \
 $(PROJECT_ROOT)/code/cbd_q_h.v  \
 $(PROJECT_ROOT)/code/rgb2ycbcr.v  \
 $(PROJECT_ROOT)/code/yd_q_h.v  \
 $(PROJECT_ROOT)/code/crd_q_h.v  \
 $(PROJECT_ROOT)/code/cr_huff.v  \
 $(PROJECT_ROOT)/code/cr_quantizer.v  \
 $(PROJECT_ROOT)/code/y_quantizer.v  \
 $(PROJECT_ROOT)/code/y_dct.v  \
 $(PROJECT_ROOT)/code/cb_huff.v  \
 $(PROJECT_ROOT)/code/y_huff.v  \
 $(PROJECT_ROOT)/code/cr_dct.v  \
 $(PROJECT_ROOT)/code/cb_quantizer.v  \
 $(PROJECT_ROOT)/code/cb_dct.v
GUI=0
SIM=icarus
COMPILE_ARGS += -DCOCOTB
COMPILE_ARGS += -DTRACE
COMPILE_ARGS += -I$(PROJECT_ROOT)
SIM_ARGS=-fst
CUSTOM_COMPILE_DEPS = $(PROJECT_ROOT)/IVERILOG_INCLUDE.v
CUSTOM_COMPILE_DEPS += $(PROJECT_ROOT)/IVERILOG_INCLUDE.v
COCOTB_ANSI_OUTPUT=1
COCOTB=/home/eyesis/git/vdt/cocotb
include $(COCOTB)/makefiles/Makefile.inc
include $(COCOTB)/makefiles/Makefile.sim
clean::
	-@rm -f *.pyc results.xml 
	-@rm -f *.jpg
