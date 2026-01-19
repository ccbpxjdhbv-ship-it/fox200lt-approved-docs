# FOX200LT Liquid Nitrogen Testing – Operating Procedure & Safety Controls

Source: Internal engineering procedure (EHS review draft)  
Document type: Operating & Safety Procedure (LN₂)  
Status: Draft – pending EHS concurrence  
Note: Text-native source for indexing and reference.
FOX200LT Liquid Nitrogen Testing – Operating Procedure & Safety Controls 

Scope note: This document is based ONLY on the FOX200LT manuals and their stated operating intent. Configuration-specific controls (e.g., hose routing, labeling, monitoring hardware) will be documented separately if needed.
0) Safety Warnings (Read Before Operating)
•	Liquid nitrogen supply required; do not run without LN₂ connected and the flow valve open. Typical Dewar line pressure ≈ 340 kPa (50 psi). (FOX200LT Instrument Manual, §1.1 Quick Start, p.3–4; §6 Low Temperature Operation, p.17)
•	Prevent condensation/ice: Do not open the test chamber during or immediately after low temperature runs. Bring plates to ~30 °C for ≥30 min before opening. (FOX200LT Instrument Manual, §1.1 Quick Start, p.3; §6 Low Temperature Operation, p.17)
•	Ventilation and oxygen displacement hazard: Operate in a well ventilated room; route nitrogen gas exhaust if ventilation is poor. (FOX200LT Instrument Manual, §6 Low Temperature Operation, p.18)
•	Dry gas purge input: Purge/dry the chamber using gas output from the LN₂ Dewar at very low positive pressure via a flow control valve similar to TIG welding. (FOX200LT Instrument Manual, §6 Low Temperature Operation, p.18)
•	Finish runs near room temperature to reduce risk of brittle components. (FOX200LT Instrument Manual, §4 Program Flow – Running a Test, p.10; §6 Low Temperature Operation, p.17–18)
•	Dry between tests: Upper +50 °C, Lower +30 °C, ≥2 mm air gap, valves OFF during drying, then ON before next test. (FOX200LT Instrument Manual, §6.1 Drying the Instrument, p.20)
•	Valve override usage: Override switch (front) ON during tests, OFF during service. (FOX200LT Instrument Manual, §6.2 Override Switch, p.20)
•	General caution: Nitrogen can be deadly if it replaces oxygen; manage exhaust appropriately. (FOX200LT Instrument Manual, §6.2 Override Switch – caution box, p.20)
Additional configuration specific controls are documented separately.
________________________________________
1) Step by Step Operating Process for Liquid Nitrogen Testing
A. Pre Start (Instrument & Environment)
1.	Verify ventilation and LN₂ supply
o	Confirm Dewar connected, valves open, typical line pressure ≈ 340 kPa (50 psi). (FOX200LT Instrument Manual, §6 Low Temperature Operation, p.17–18)
2.	Power on instrument; unit warm and dry
o	If recently operated at low temp or idle long period, perform drying cycle: Upper +50 °C, Lower +30 °C, ≥2 mm gap, valves OFF for ≥ a couple of hours; then valves ON before next test. (FOX200LT Instrument Manual, §6.1 Drying the Instrument, p.20)
3.	Do not open chamber at extreme cold
o	Warm plates to ~30 °C for ≥30 min before opening after low temp work. (FOX200LT Instrument Manual, §1.1 Quick Start, p.3)
4.	Set valve override
o	ON during tests; OFF during service. (FOX200LT Instrument Manual, §6.2 Override Switch, p.20)
B. Instrument Setup (Local Keypad)
5.	Select units (SI or English)
o	(FOX200LT Instrument Manual, §4 Program Flow – Screen 1, p.7)
6.	Open stack and calibrate thickness (Delta X)
o	Clean plates; Open Stack / Calibrate Delta X to zero thickness. (FOX200LT Instrument Manual, §4 Program Flow – Screen 2, p.8)
7.	Select calibration type
o	NIST 1450b SRM (typical) or User Type per saved calibration. (FOX200LT Instrument Manual, §4 Program Flow – Screen 3–4, p.8)
8.	Test mode selection and setpoints
o	Test (not Calibration), do not maintain temperature between tests on FOX200LT to avoid LN₂ waste. (FOX200LT Instrument Manual, §4 Program Flow – Screen 5, p.9)
o	Enter upper/lower plate setpoints (up to 9 pairs). Heat flow up; ΔT typically 20 °C; negative temperature entry via 0 then digits. (FOX200LT Instrument Manual, §4 Program Flow – Screen 6, p.9–10; §3 Pre Saved Calibration, p.6–7)
9.	Insert sample; thickness mode
o	Auto Thickness (rigid) or User Defined Thickness (compressible); actual spacing displayed; enter Sample ID to start. (FOX200LT Instrument Manual, §4 Program Flow – Screen 7–8, p.11; Screen 8–11, p.11–12)
C. PC Assisted Operation (WinTherm32) – If Using Computer
10.	Establish communication
o	Aux → Port → Enable COM/USB (as applicable); confirm FOX Instrument – COM# window with live readings. (WinTherm32 Software Manual, §4.1 Establishing Communication, p.15–16; §4.2 Application and COM window, p.17–19)
11.	Start test from PC (optional)
o	Run → Start → Start Test Run; Test Mode: Normal, select 1450b calibration (filed/computer or instrument), Auto/Manual thickness, then Run. (WinTherm32 Software Manual, §4 “WinTherm32” Run – Start Test Run window, p.16; §2 Quick Start of Tests, p.7–11)
12.	Enter Sample Information and Setpoints
o	Name, thickness, Aux Info; enter setpoints (Upper/Lower or Mean/Delta). (Quick Start on Computer, Steps 4–5; WinTherm32 Software Manual, §5.3.1 Sample; §5.3.2 Setpoints, p.31–33)
13.	Monitoring & Equilibrium
o	Observe U/L temperatures, QU/QL signals, block counter, and equilibrium indicators: $ (TE), * (SE), % (PE). (FOX200LT Instrument Manual, §4 Program Flow – Screen 9–10, p.11–12; §5 Data Organization and Equilibrium Criteria, p.16–17)
14.	Results
o	Results per setpoint: λU and λL; use the average. (FOX200LT Instrument Manual, §4 Program Flow – Screen 10, p.12)
15.	End of test / repeat
o	Choose to repeat at same temperatures or enter new; do not maintain low temps between tests on FOX200LT. (FOX200LT Instrument Manual, §4 Program Flow – Screen 11, p.12–13; Screen 5 guidance, p.9)
D. Post Run Drying & Shutdown
16.	Dry the instrument between tests
o	Upper +50 °C, Lower +30 °C, ≥2 mm gap; valves OFF during drying; run ≥ a couple of hours; turn valves ON before next test. (FOX200LT Instrument Manual, §6.1 Drying the Instrument, p.20)
17.	Do not open chamber cold
o	Warm to ~30 °C for ≥30 min before opening. (FOX200LT Instrument Manual, §1.1 Quick Start, p.3)
Additional configuration specific controls are documented separately.
________________________________________
2) Potential Failure or Upset Conditions (Identification)
•	Temperature runaway / overheating or setpoint not reached
o	Monitor plate temperatures; WinTherm32 “Use plate overheat check” option exists and setpoint reach checks are available; if setpoints are not reached within defined hours the setpoint is skipped. (WinTherm32 Software Manual, §4.3 Test Setup – More… Test Options, p.23–24)
•	Condensation/Ice formation
o	Occurs if chamber door is opened during/after low temperature runs; avoid opening, use Condensation Reset Button (rear) to activate heaters raising chassis to room temp. (FOX200LT Instrument Manual, §6 Low Temperature Operation, p.18)
•	Insufficient LN₂ flow or valve state
o	Override switch must be ON during tests; OFF during service; ensure valves ON before tests and OFF during drying. (FOX200LT Instrument Manual, §6.2 Override Switch, p.20; §6.1 Drying, p.20)
•	Equilibrium not achieved / prolonged run
o	Equilibrium criteria (TE/SE/PE, number of blocks, inflexion) govern completion; thicker/compressible samples may require more time. (FOX200LT Instrument Manual, §5 Equilibrium Criteria, p.16–17; WinTherm32 Software Manual, §2 Quick Start criteria notes, p.11)
•	Communication issues (PC ↔ instrument)
o	COM/USB port selection and enable; use Aux → Port → Reset Port if needed. (WinTherm32 Software Manual, §4.1; §5.6 Aux commands, p.40)
Additional configuration specific controls are documented separately.
________________________________________
3) Actions in the Event of a Leak, Line Failure, or Unexpected Nitrogen Release
Safety focus first; follow site emergency protocols.
•	Immediate actions
o	Do not open the test chamber at extreme low temperatures; prioritize preventing condensation/ice damage. (FOX200LT Instrument Manual, §1.1 Quick Start, p.3)
o	Recognize oxygen displacement hazard: nitrogen can replace oxygen; ensure area ventilation and manage exhaust routing per configuration. (FOX200LT Instrument Manual, §6 Low Temperature Operation – exhaust routing and ventilation, p.18; §6.2 caution, p.20)
•	Instrument controls
o	Turn valve override OFF (front) if servicing/state isolation is required; turn LN₂ valves OFF (rear button) as appropriate to stop LN₂ flow. (FOX200LT Instrument Manual, §6.2 Override Switch, p.20; §6.1 Drying – valves OFF instruction, p.20)
•	Purge and drying as recovery
o	After stabilization, employ dry gas purge input at very low positive pressure via flow control valve similar to TIG to purge/dry the chamber; execute standard drying cycle (Upper +50 °C / Lower +30 °C, ≥2 mm gap). (FOX200LT Instrument Manual, §6 Low Temperature Operation, p.18; §6.1 Drying, p.20)
•	Ventilation management
o	Operate in well ventilated area and route exhaust gas appropriately to avoid oxygen depletion; do not allow liquid nitrogen in exhaust; aim for gas only exhaust. (FOX200LT Instrument Manual, §6 Low Temperature Operation – exhaust guidance, p.18)
Additional configuration specific controls are documented separately.
________________________________________
4) Roles and Responsibilities (Normal Operation & Emergency Response)
A. Normal Operation (Technicians)
•	Pre run safety checks
o	Verify LN₂ supply and valves ON; confirm ventilation; prepare for drying if needed. (FOX200LT Instrument Manual, §6, p.17–18; §6.1, p.20)
•	Instrument setup
o	Units selection; thickness zeroing (Calibrate Delta X); calibration type; test setpoints; sample insertion; equilibrium monitoring. (FOX200LT Instrument Manual, §4 Program Flow Screens 1–11, p.7–13)
•	Post run drying & shutdown
o	Execute drying (Upper +50 °C / Lower +30 °C, ≥2 mm gap; valves OFF during drying, ON before next test). (FOX200LT Instrument Manual, §6.1, p.20)
•	PC operation (if used)
o	Establish COM/USB; configure test; monitor equilibrium and results; manage calibration selection. (WinTherm32 Software Manual, §4.1–4.3, p.15–24; §2, p.7–11)
B. Emergency Response (Technicians; coordinated with EHS)
•	Immediate control measures
o	Valve override OFF as needed; LN₂ valves OFF to isolate LN₂ supply; maintain ventilation. (FOX200LT Instrument Manual, §6.2, p.20; §6.1, p.20; §6, p.18)
•	Stabilize instrument
o	Avoid opening chamber at low temperature; when safe, use Condensation Reset Button and drying cycle to restore to room temperature conditions. (FOX200LT Instrument Manual, §6, p.18; §6.1, p.20)
•	Communications & documentation
o	Report event per facility protocol; record setpoints, valve states, purge operations, and timing.
C. Roles and Responsibilities
Responsible Engineer (Name: ___________)
•	Owns the test plan and ensures procedures and controls are current
•	Confirms configuration matches the approved setup (purge line, sleeving, venting/ventilation approach, signage, log sheet)
•	Reviews results and maintains test records
Engineering Technician / Operator (Name: ___________)
•	Executes testing per procedure (startup, run, shutdown, drying)
•	Uses required PPE and completes pre-run safety checks
•	Monitors conditions during testing and isolates/stops the system if abnormal conditions occur
•	Completes time-in/time-out log and posts/removes door signage per session
EHS Reviewer (Name: ___________) (optional, recommended for initial run)
•	Reviews safety controls and documentation
•	Observes initial calibration/testing if desired
•	Provides feedback for final approval
Additional configuration specific controls are documented separately if necessary.
Sources Ledger
•	FOX200LT Instrument Manual (Rev 5b)
o	§1.1 Quick Start (p.3–4)
o	§3 Pre Saved Calibration (p.6–7)
o	§4 Program Flow – Screens 1–11 (p.7–13)
o	§5 Data Organization & Equilibrium Criteria (p.16–17)
o	§6 Low Temperature Operation (p.17–19) 
	Dry gas purge input; exhaust/ventilation guidance; Dewar pressure; Condensation Reset Button (p.18–19)
o	§6.1 Drying the Instrument (p.20)
o	§6.2 Override Switch for Valves (p.20)
•	WinTherm32 Software Manual (+ Addendum for FOX200LT)
o	§2 Quick Start of Tests (p.7–11)
o	§4.1 Establishing Computer Instrument Communication (p.15–16)
o	§4.2 WinTherm32 Application & COM window (p.17–19)
o	§4.3 Test Setup & More… Test Options (p.20–24)
o	§5.6 Aux Commands (Port/Reset) (p.40)
•	Quick Start on Computer (PDF)
o	COM Port setup; Start Test Run; Sample Information; Setpoints windows (page content)
Document Control / Status
•	Document title: FOX200LT Liquid Nitrogen Testing – Operating Procedure & Safety Controls (EHS Draft)
•	Prepared by: Engineering
•	Intended use: EHS review and approval for calibration and testing
•	Scope limitation: This document reflects manufacturer manuals and verified operating intent. Configuration-specific hardware controls are documented separately if required.
•	Revision status: Draft – pending EHS review and initial calibration observation
•	Effective date: TBD upon EHS concurrence
