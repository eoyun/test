# notice
## test
daq operation

    cd test/TB_daq 
    ./run_all.sh (config) (number of events)`

config file 

TCB board

    cat config/setup/set_TCB.txt

    cw_tcb 10
    ptrigger_interval 0
    trig_enable 8
    mthr_tcb 1
    prescale 1

cw_tcb : coincidence width in TCB board
ptrigger_interval : time interval of pedestal trigger (ms)
trig_enable : select the trigger ( 1: self trigger, 2: pedestal trigger, 4: software trigger, 8: external trigger)
mthr_tcb : multiplicity threshold in TCB board
prescale : prescale of waveform mode

DAQ board

    cat config/setup/set_DAQ_1.txt

    cw_daq 5
    hv 0.0 0.0 0.0 0.0
    mthr_daq 1
    trig_latancy 250
    trig_dly 0
    down_sampling 0
    pulse_width 250
    risetime 120
    fraction 0.3
    peak_srch_dly 0 0 0 0
    peak_srch_wth 1000 1000 1000 1000
    thr
    4095 4095 4095 4095 4095 4095 4095 4095
    4095 4095 4095 4095 4095 4095 4095 4095
    4095 4095 4095 4095 4095 4095 4095 4095
    4095 4095 4095 4095 4095 4095 4095 4095

## programmer
daq firmware upgrade
