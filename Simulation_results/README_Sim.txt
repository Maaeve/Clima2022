The development of the simulation model was carried out for a single outdoor temperature, namely 8 °C.
The validated heat pump model was then simulated for two different outdoor temperatures, namely 0 °C and 8 °C. 
For the energy analysis, the validated heat pump model with an outdoor temperature of 8 °C used experimental measurements of the domestic hot water inlet and evaporator inlet temperature as inputs instead of using fixed temperature inputs. 
Such an approach with experimental measurements as inputs allowed to address the variability in supply temperature from the laboratory for the evaporator and domestic hot water inlet side.

Hence, in total 5 different simulation results can be found:
- Heat pump model with start parameters at an outdoor temperature of 8 °C (file: SimData_Tout_8_degrees_StartModel)
- Heat pump model with improvements at controllers for compressor, condenser pump and domestic hot water at an outdoor temperature of 8 °C (file: SimData_Tout_8_degrees_ImprovedModel)
- Extends from improved heat pump model and further implements the evaporator pump control to reach a validated, final heat pump model at an outdoor temperature of 8 °C (file: SimData_Tout_8_degrees_ValidatedModel)
- Uses the validated, final heat pump model, but at an outdoor temperature of 0 °C (file: SimData_Tout_0_degrees_ValidatedModel)
- Uses the validated, final heat pump model, at an outdoor temperature of 8 °C and with the experimental measurements of the domestic hot water inlet and evaporator inlet temperature as inputs instead of using constant inputs (file: SimData_Tout_8_degrees_ValidatedModel_ExperimentalInputs)

The used acronyms within the simulation result file with related meanings and units are:

Acronym	Meaning	Unit

Time	Time	s
Evap.m_flow	Evaporator flow rate	kg/s
Cond.m_flow	Condenser flow rate	kg/s
Compressor	Compressor status	binary
Comp.P_el	Electric compressor power according heat pump black box model	W
Comp.P_evap	Evaporator power according heat pump black box model	W
Comp.P_cond	Condenser power according heat pump black box model	W
Comp.T_evap_in	Evaporator inlet temperature	K
Comp.T_evap_out	Evaporator outlet temperature	K
Comp.T_cond_in	Condenser inlet temperature	K
Comp.T_cond_out	Condenser outlet temperature (before back-up heater)	K
Comp.T_cond_set	Condenser outlet temperature setpoint	K
SH_load.T_in	Space heating load inlet temperature	K
SH_load.T_out	Space heating load outlet temperature	K
SH_load.TSet	Space heating load outlet temperature setpoint	K
SH_load.Power	Extracted space heating power via virtual load	W
SH_load.Energy	Extracted cumulative space heating energy via virtual load	kWh
TES2.T_out	System inertia tank outlet temperature	K
3way..m_flow_in	Inlet flow rate from condenser	kg/s
3way.m_flow_DHW	Outlet flow rate to domestic hot water	kg/s
3way.m_flow_SH	Outlet flow rate to space heating	kg/s
3way.pos_real	Three-way valve position with 0 = position domestic hot water and 1 = position space heating	-
Toutdoor	Outdoor temperature 	K
BUH.power	Thermal and electrical power of back-up heater as conversion efficiency is 100 %	W
BUH.T_out	Back-up heater outlet temperature	K
Pump_cond.mod_mea	Measured modulation speed of condenser pump with 0 = off and 1 = full load	-
Pump_cond.power	Electricity consumption condenser pump	W
Pump_evap.mod_mea	Measured modulation speed of evaporator pump with 0 = off and 1 = full load	-
Pump_evap.power	Electricity consumption evaporator pump	W
DHW.T_cold_in	Cold water inlet temperature of domestic hot water storage	K
DHW.T_hot_out	Hot water outlet temperature of domestic hot water storage	K
DHW.m_flow	Extracted domestic hot water flow rate	kg/s
DHW.T_layer_1	Temperature of domestic hot water storage layer 1 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_2	Temperature of domestic hot water storage layer 2 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_3	Temperature of domestic hot water storage layer 3 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_4	Temperature of domestic hot water storage layer 4 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_5	Temperature of domestic hot water storage layer 5 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_6	Temperature of domestic hot water storage layer 6 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_7	Temperature of domestic hot water storage layer 7 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_8	Temperature of domestic hot water storage layer 8 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_9	Temperature of domestic hot water storage layer 9 with storage top = layer 1 and storage bottom = layer 10	K
DHW.T_layer_10	Temperature of domestic hot water storage layer 10 with storage top = layer 1 and storage bottom = layer 10	K
VDHW	Cumulative extracted domestic hot water volume	l
Total.P_el	Total heat pump electrical power	W
Total.E_el	Total cumulative heat pump electrical energy	kWh
Legio.T_DHW_Low_Set	Domestic hot water lower hysteresis temperature	K
Legio.T_DHW_High_Set	Domestic hot water upper hysteresis temperature	K
Legio.Status	Activation of anti-legionella cycle	binary
DHW_thermostat.status	Domestic hot water activation request signal	binary
Control.Tsupply_Set_BUH	Requested supply temperature of back-up heater, to be confirmed by internal back-up heater controller	K
Control.Tsupply_Set_HP	Requested supply temperature of compressor, to be confirmed by internal compressor controller	K
Pel_standby	Constant electricity consumption of heat pump as standby power	W
Comp.E_evap	Cumulative evaporator energy according heat pump black box model	kWh
Comp.E_cond	Cumulative condenser energy according heat pump black box model	kWh
Comp.E_el	Cumulative electric compressor energy according heat pump black box model	kWh
BUH.E_el	Cumulative back-up heater energy according heat pump black box model	kWh
Comp.On_off_Req	Requested compressor status after modulation controller as input to runtime controller	binary
Comp.On_off_Ack	Acknowledged compressor status after modulation controller and after approval of runtime controller	binary
