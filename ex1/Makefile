TARGET = test
FILES = ff_tb.v d_f.v t_ff.v rcc.v

all: $(TARGET)

$(TARGET): $(FILES)
	iverilog -o $(TARGET) $(FILES)

run: $(TARGET)
	vvp test

wave: run
	gtkwave test.vcd &

clean:
	rm $(TARGET) $(TARGET).vcd
