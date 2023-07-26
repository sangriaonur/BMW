# BMW
FDL Codes
<?xml version="1.0" encoding="utf-8"?>
<FDL>
    <!--SaNGRia-->
    <cafd id="000017BE" name="BDC_01" author="SaNGRia" series="F015">
        <code description="ENABLE  Electronic (Radio and Nav) SHUTOFF when drivers door opened">
            <group id="3020">
                <function start="9" end="9" comment="TCM_LOGIC_R_OFF_DOOR" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Electronic (Radio and Nav) SHUTOFF when drivers door opened">
            <group id="3020">
                <function start="9" end="9" comment="TCM_LOGIC_R_OFF_DOOR" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Door Handle LED Lights while in reverse">
            <group id="3070">
                <function start="128" end="128" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE FRONT driver/passenger window Roll Up when doors opened">
            <group id="3050">
                <function start="0" end="0" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE REAR driver/passenger window Roll Up when doors opened">
            <group id="3051">
                <function start="0" end="0" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Open/Close windows and mirrors via keyFOB - CA (NA Cars)">
            <group id="3056">
                <function start="0" end="0" mask="01000000b">aktiv</function>
                <function start="0" end="0" mask="10000000b">aktiv</function>
                <function start="1" end="1" mask="00000100b">aktiv</function>
                <function start="1" end="1" mask="00000001b">aktiv</function>
                <function start="1" end="1" mask="00000010b">aktiv</function>
            </group>
            <group id="3110">
                <function start="0" end="0" mask="10000000b">aktiv</function>
                <function start="7" end="7" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="Remove open/close window and mirror initiation delay">
            <group id="3056">
                <function start="10" end="10" mask="11111111b">00</function>
            </group>
        </code>
        <code description="Unlock doors when STOP engine (Older I-Step)">
            <group id="3040">
                <function start="2" end="2" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="Unlock doors when STOP engine - auto-locked (Newer I-Step)">
            <group id="3041">
                <function start="40" end="40" comment="CLI_DEFAULT_UNLOCK_AFTER_END_OF_DRIVING" mask="00000011b">nur_nach_v_verriegeln</function>
            </group>
        </code>
        <code description="Unlock doors when STOP engine - auto or manual lock (Newer I-Step)">
            <group id="3041">
                <function start="40" end="40" comment="CLI_DEFAULT_UNLOCK_AFTER_END_OF_DRIVING" mask="00000011b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Engine Start Without Holding Brake) (EXCLUDES I3)">
            <group id="3020">
                <function start="8" end="8" comment="TCM_STARTLOCK_BRAKE" mask="00000001b">nicht_aktiv</function>
                <function start="8" end="8" comment="TCM_STARTLOCK_DRIVINGREADINESS" mask="00010000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Front and Rear DRL (8TL)">
            <group id="3068">
                <function start="31" end="31" mask="00110000b">drl_s</function>
            </group>
            <group id="3064">
                <function start="221" end="221" mask="00111111b">sl_l</function>
                <function start="234" end="234" mask="00111111b">sl_r</function>
            </group>
            <group id="3065">
                <function start="78" end="78" mask="00111111b">sl_2_l</function>
                <function start="91" end="91" mask="00111111b">sl_2_r</function>
            </group>
        </code>
        <code description="F15 - ENABLE Variable Light Distribution (VLD)">
            <group id="3073">
                <function start="40" end="42" mask="11111111b">9C, 9C, 9C</function>
                <function start="152" end="152" mask="00000001b">F015ENABLE</function>
            </group>
        </code>
        <code description="DISABLE Auto Start/Stop (ASS) at every startup (Comfort Mode)">
            <group id="3023">
                <function start="0" end="0" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Auto Start/Stop (ASS) at every startup (Eco Pro Mode)">
            <group id="3023">
                <function start="1" end="1" mask="00001100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Auto Start/Stop (ASS) Remembers Last Setting (ON or OFF)">
            <group id="3023">
                <function start="0" end="0" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Reduced Rain HeadLight Sensor Sensitivity (Insensitive)">
            <group id="3130">
                <function start="5" end="5" mask="00000111b">unempfindlich</function>
            </group>
        </code>
        <code description="DISABLE Horn Lock Confirmation with Engine On">
            <group id="3040">
                <function start="0" end="0" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Horn Lock Confirmation with Engine On">
            <group id="3040">
                <function start="0" end="0" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="Change Number of Soft Turn Signal Blinks to 5 (Old I-STEP, Less than 3.59)">
            <group id="3068">
                <function start="7" end="7" comment="See Newer Coding if F025-16-07-501" mask="00000111b">04</function>
            </group>
        </code>
        <code description="Change Number of Soft Turn Signal Blinks to 5 (New I-STEP, Greater then 3.59.x)">
            <group id="3069">
                <function start="215" end="215" comment="Firmware F025-16-07-501, 00 = 1, 01 = 3, 02 =5" mask="00011000b">02</function>
            </group>
        </code>
        <code description="ENABLE Increased Passenger Mirror Tilt (Curb View) in Reverse">
            <group id="3110">
                <function start="1" end="1" mask="11111111b">5A</function>
            </group>
        </code>
        <code description="Removes Trunk Open Delay (Instant) via KeyFOB">
            <group id="30D0">
                <function start="18" end="18" mask="11111111b">wert_00</function>
            </group>
        </code>
        <code description="ENABLE Increased Side Mirror Dimming (Tinted Windows)">
            <group id="3120">
                <function start="23" end="23" comment="left mirror" mask="11111100b">39</function>
                <function start="30" end="30" comment="right mirror" mask="11111100b">39</function>
            </group>
        </code>
        <code description="F015 - ENABLE EU Brake Force Display (BFD) Light Behavior (Blink)">
            <group id="3068">
                <function start="16" end="16" comment="Default USA = glow brighter and wider" mask="00000011b">02</function>
            </group>
            <group id="3064">
                <function start="156" end="156" comment="MAPPING_BRAKEFORCED_1_L_OUTPUT" mask="00111111b">18</function>
                <function start="169" end="169" comment="MAPPING_BRAKEFORCED_1_R_OUTPUT" mask="00111111b">19</function>
            </group>
            <group id="3065">
                <function start="52" end="52" comment="MAPPING_BRAKEFORCED_2_L_OUTPUT" mask="00111111b">14</function>
                <function start="65" end="65" comment="MAPPING_BRAKEFORCED_2_R_OUTPUT" mask="00111111b">15</function>
            </group>
        </code>
        <code description="F015 - ENABLE EU Brake Force Display (BFD) (Additional Settings) (TESTING)">
            <group id="3064">
                <function start="158" end="158" comment="MAPPING_BRAKEFORCED_1_L_PRIORITY" mask="11100000b">01</function>
                <function start="159" end="159" comment="MAPPING_BRAKEFORCED_1_L_PWM_1_BFD" mask="11111111b">64</function>
                <function start="162" end="162" comment="MAPPING_BRAKEFORCED_1_L_PWM_4" mask="11111111b">00</function>
                <function start="165" end="165" comment="MAPPING_BRAKEFORCED_1_L_DEPENDENCY_FUNC" mask="00011111b">00</function>
                <function start="171" end="171" comment="MAPPING_BRAKEFORCED_1_R_PRIORITY" mask="11100000b">01</function>
                <function start="172" end="172" comment="MAPPING_BRAKEFORCED_1_R_PWM_1_BFD" mask="11111111b">64</function>
                <function start="175" end="175" comment="MAPPING_BRAKEFORCED_1_R_PWM_4" mask="11111111b">00</function>
                <function start="178" end="178" comment="MAPPING_BRAKEFORCED_1_R_DEPENDENCY_FUNC" mask="00011111b">00</function>
            </group>
            <group id="3065">
                <function start="54" end="54" comment="MAPPING_BRAKEFORCED_2_L_PRIORITY" mask="11100000b">01</function>
                <function start="55" end="55" comment="MAPPING_BRAKEFORCED_2_L_PWM_1_BFD" mask="11111111b">64</function>
                <function start="56" end="56" comment="MAPPING_BRAKEFORCED_2_L_PWM_2_ESS_1" mask="11111111b">00</function>
                <function start="57" end="57" comment="MAPPING_BRAKEFORCED_2_L_PWM_3_ESS_2" mask="11111111b">00</function>
                <function start="58" end="58" comment="MAPPING_BRAKEFORCED_2_L_PWM_4" mask="11111111b">64</function>
                <function start="67" end="67" comment="MAPPING_BRAKEFORCED_2_R_PRIORITY" mask="11100000b">01</function>
                <function start="68" end="68" comment="MAPPING_BRAKEFORCED_2_R_PWM_1_BFD" mask="11111111b">64</function>
                <function start="69" end="69" comment="MAPPING_BRAKEFORCED_2_R_PWM_2_ESS_1" mask="11111111b">00</function>
                <function start="70" end="70" comment="MAPPING_BRAKEFORCED_2_R_PWM_3_ESS_2" mask="00111111b">00</function>
                <function start="71" end="71" comment="MAPPING_BRAKEFORCED_2_R_PWM_4" mask="00011111b">64</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Short Press = No Action)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_SHORT" mask="00001111b">00</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Short Press = Open Trunk)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_SHORT" mask="00001111b">02</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Short Press = Panic Alarm)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_SHORT" mask="00001111b">03</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Short Press = Follow-Me-Home)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_SHORT" mask="00001111b">04</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Short Press = Open Frunk - Front Boot)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_SHORT" mask="00001111b">05</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Short Press = Auxillary Cooling)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_SHORT" mask="00001111b">07</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Medium Press = No Action)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_MID" mask="11110000b">00</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Medium Press = Open Trunk)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_MID" mask="11110000b">02</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Medium Press = Panic Alarm)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_MID" mask="11110000b">03</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Medium Press = Follow-Me-Home)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_MID" mask="11110000b">04</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Medium Press = Open Frunk - Front Boot)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_MID" mask="11110000b">05</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Medium Press = Auxillary Cooling)">
            <group id="30D0">
                <function start="13" end="13" comment="RC_DEFAULT_IDG_3RD_BUTTON_MID" mask="11110000b">07</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Long Press = No Action)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_3RD_BUTTON_LONG" mask="00001111b">00</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Long Press = Open Trunk)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_3RD_BUTTON_LONG" mask="00001111b">02</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Long Press = Panic Alarm)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_3RD_BUTTON_LONG" mask="00001111b">03</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Long Press = Follow-Me-Home)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_3RD_BUTTON_LONG" mask="00001111b">04</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Long Press = Open Frunk - Front Boot)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_3RD_BUTTON_LONG" mask="00001111b">05</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 3RD Button (Long Press = Auxillary Cooling)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_3RD_BUTTON_LONG" mask="00001111b">07</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Short Press = No Action)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_4TH_BUTTON_SHORT" mask="11110000b">00</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Short Press = Open Trunk)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_4TH_BUTTON_SHORT" mask="11110000b">02</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Short Press = Panic Alarm)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_4TH_BUTTON_SHORT" mask="11110000b">03</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Short Press = Follow-Me-Home)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_4TH_BUTTON_SHORT" mask="11110000b">04</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Short Press = Open Frunk - Front Boot)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_4TH_BUTTON_SHORT" mask="11110000b">05</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Short Press = Auxillary Cooling)">
            <group id="30D0">
                <function start="14" end="14" comment="RC_DEFAULT_IDG_4TH_BUTTON_SHORT" mask="11110000b">07</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Medium Press = No Action)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_MID" mask="00001111b">00</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Medium Press = Open Trunk)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_MID" mask="00001111b">02</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Medium Press = Panic Alarm)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_MID" mask="00001111b">03</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Medium Press = Follow-Me-Home)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_MID" mask="00001111b">04</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Medium Press = Open Frunk - Front Boot)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_MID" mask="00001111b">05</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Medium Press = Auxillary Cooling)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_MID" mask="00001111b">07</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Long Press = No Action)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_LONG" mask="11110000b">00</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Long Press = Open Trunk)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_LONG" mask="11110000b">02</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Long Press = Panic Alarm)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_LONG" mask="11110000b">03</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Long Press = Follow-Me-Home)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_LONG" mask="11110000b">04</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Long Press = Open Frunk - Front Boot)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_LONG" mask="11110000b">05</function>
            </group>
        </code>
        <code description="Change Behavior of keyFOB 4TH Button (Long Press = Auxillary Cooling)">
            <group id="30D0">
                <function start="15" end="15" comment="RC_DEFAULT_IDG_4TH_BUTTON_LONG" mask="11110000b">07</function>
            </group>
        </code>
        <code description="ENABLE Ambiance Lighting controlled independent from Dimmer Switch">
            <group id="3070">
                <function start="135" end="135" comment="AMBIENTE_NACHFUEHRUNG" mask="10000000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Ambiance Lighting controlled independent from Dimmer Switch">
            <group id="3070">
                <function start="135" end="135" comment="AMBIENTE_NACHFUEHRUNG" mask="10000000b">01</function>
            </group>
        </code>
        <code description="Turn on Fog Lights with Welcome Lights - SOFT ON">
            <group id="3063">
                <function start="66" end="66" comment="MAPPING_NEBELSCHW_L_PART_OF" mask="11111111b">01</function>
                <function start="79" end="79" comment="MAPPING_NEBELSCHW_R_PART_OF" mask="11111111b">01</function>
            </group>
        </code>
        <code description="Turn on Fog Lights with Follow-Me-Home, or Alarm - HARD ON">
            <group id="3063">
                <function start="66" end="66" comment="MAPPING_NEBELSCHW_L_PART_OF" mask="11111111b">10</function>
                <function start="79" end="79" comment="MAPPING_NEBELSCHW_R_PART_OF" mask="11111111b">10</function>
            </group>
        </code>
        <code description="ENABLE Heated Steering Wheel Instrument Cluster Status">
            <group id="3140">
                <function start="18" end="18" comment="LHZ_CCM" mask="01000000b">01</function>
            </group>
        </code>
        <code description="ENABLE DARK REAR WINDOW - MIRROR DIMMING">
            <group id="3120">
                <function start="3" end="3" comment="ISP_HECKSCHEIBE" mask="00000110b">01</function>
            </group>
        </code>
        <code description="ENABLE LIGHT REAR WINDOW - MIRROR DIMMING">
            <group id="3120">
                <function start="3" end="3" comment="ISP_HECKSCHEIBE" mask="00000110b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000092" name="IHKA_CBF" author="SaNGRia" series="F015,F010">
        <code description="ENABLE HVAC memory - A/C stay OFF if OFF at vehicle shutdown">
            <group id="3000">
                <function start="5" end="5" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Air Re-Circulation memory - Remembers shutdown Setting">
            <group id="3000">
                <function start="0" end="0" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE A/C from turning ON if Auto Button is pressed">
            <group id="3000">
                <function start="5" end="5" mask="00001000b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="000047D6" name="IHKA2" author="SaNGRia" series="F015">
        <code description="ENABLE HVAC memory - A/C stay OFF if OFF at vehicle shutdown">
            <group id="3000">
                <function start="5" end="5" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Air Re-Circulation memory - Remembers shutdown Setting">
            <group id="3000">
                <function start="0" end="0" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE A/C from turning ON if Auto Button is pressed">
            <group id="3000">
                <function start="5" end="5" mask="00001000b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="000016EE" name="IHKA_VA02" author="SaNGRia" series="F020,F020,I001">
        <code description="ENABLE HVAC memory - A/C stay OFF if OFF at vehicle shutdown">
            <group id="3003">
                <function start="0" end="0" comment="MEMORY_OFF" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Air Re-Circulation memory - Remembers shutdown Setting">
            <group id="3003">
                <function start="0" end="0" comment="MEMORY_UMLUFT" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE A/C from turning ON if Auto Button is pressed">
            <group id="3003">
                <function start="0" end="0" mask="00000100b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001AB7" name="PMA_PDC" author="SaNGRia" series="F015">
        <code description="ENABLE Top/Rearview Cameras at ALL speeds. See iCAM for Sideview">
            <group id="300B">
                <function start="8" end="8" comment="speed when auto disables top view" mask="11111111b">FF</function>
                <function start="9" end="9" comment="speed when auto disables rear view" mask="11111111b">FF</function>
                <function start="10" end="10" comment="distance when auto disables top view" mask="11111111b">FF</function>
                <function start="11" end="11" comment="distance when auto disables rear view" mask="11111111b">FF</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000146B" name="PMA_PDC" author="SaNGRia" series="F015,I001">
        <code description="ENABLE Top/Rear Camera at All Speeds. Part 1 of 2. See icam for Side">
            <group id="300D">
                <function start="8" end="8" comment="max speed to disables top camera view" mask="11111111b">FF</function>
                <function start="9" end="9" comment="max speed to disables rear camera view" mask="11111111b">FF</function>
                <function start="10" end="10" comment="max distance to disables top camera view" mask="11111111b">FF</function>
                <function start="11" end="11" comment="max distance to disables rear camera view" mask="11111111b">FF</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000163C" name="iCAM" author="SaNGRia" series="F015">
        <code description="ENABLE Sideview Cameras at ALL speeds">
            <group id="3006">
                <function start="1" end="1" comment="Activate SV at any speed - part 1" mask="11111111b">FF</function>
                <function start="2" end="2" comment="Activate SV at any speed - part 2" mask="11111111b">FF</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001148" name="KAFAS2" author="SaNGRia" series="F010,F015">
        <code description="ENABLE Grass/Roadside Edge detection to Lane Departure">
            <group id="3020">
                <function start="2" end="2" mask="00000011b">detection_for_grass_edge_and_curb_stone</function>
            </group>
        </code>
        <code description="ENABLE EU SLI sign (White circle with Red outline)">
            <group id="3010">
                <function start="1" end="1" mask="01111000b">ECE_white</function>
            </group>
        </code>
        <code description="ENABLE HUD Distance Info (Part 3 of 3. See KOMBI and KAFAS2)">
            <group id="3060">
                <function start="1" end="1" comment="werte=01" mask="00000010b">IBRAKE_STAT_on_F010</function>
                <function start="1" end="1" comment="werte=01" mask="00000100b">F010</function>
                <function start="1" end="1" comment="werte=01" mask="00011000b">01</function>
            </group>
        </code>
        <code description="DISABLE HUD Distance Info (Part 3 of 3. See KOMBI and KAFAS2)">
            <group id="3060">
                <function start="1" end="1" comment="SEND_STATUS_IBRAKE" mask="00000010b">00</function>
                <function start="1" end="1" comment="SEND_PARAM_IBRAKE" mask="00000100b">01</function>
                <function start="1" end="1" comment="DISPLAY_HEADWAY_DISTANCE" mask="00011000b">00</function>
            </group>
        </code>
        <code description="ENABLE HUD Do Not Pass/Pass with care. Part 2 of 2. See KOMBI">
            <group id="3010">
                <function start="1" end="1" comment="NPI_ON_OFF" mask="00000010b">01</function>
            </group>
        </code>
    </cafd>
    <cafd id="000007C8" name="HKFM" author="SaNGRia" series="F001,F010,F015,F025,F030,F045">
        <code description="ENABLE Trunk Close via keyFOB/Footwell button (NA vehicles)">
            <group id="3010">
                <function start="0" end="0" mask="00001000b">aktiv</function>
                <function start="2" end="2" mask="00000100b">aktiv</function>
                <function start="2" end="2" mask="00001000b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000DED" name="HU_NBT" author="SaNGRia">
        <code description="ENABLE Call Log Timestamp">
            <group id="3003">
                <function start="1" end="1" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Entire text (SMS) message display on iDrive">
            <group id="3000">
                <function start="34" end="34" comment="MYINFO_DRIVING_TEXT_LENGTH" mask="00011100b">07</function>
                <function start="34" end="34" comment="AKD_DRIVING_TEXT_LENGTH" mask="11100000b">07</function>
                <function start="35" end="35" comment="BMWINFO_DRIVING_TEXT_LENGTH" mask="00000111b">07</function>
            </group>
            <group id="3003">
                <function start="11" end="11" comment="PIM_DRIVING_TEXT_LENGTH" mask="00000111b">07</function>
            </group>
        </code>
        <code description="ENABLE HUD Turnsignal. Part 1 of 2 - See KOMBI (Excludes 6WB DKOMBI)">
            <group id="3001">
                <function start="55" end="55" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Lock/Unlock Sound Confirm Checkbox With alarm only">
            <group id="3000">
                <function start="110" end="110" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Lock/Unlock Sound Confirm Checkbox With alarm only">
            <group id="3000">
                <function start="110" end="110" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Sports Displays. Part 1 of 2. See KOMBI">
            <group id="3000">
                <function start="101" end="101" mask="00010000b">aktiv</function>
                <function start="107" end="107" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE AM Radio on Hybrid Vehicles (F15-40e/I012/I001)">
            <group id="3002">
                <function start="52" end="52" comment="RADIO_BAND_KW" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE British Voice on Navigation">
            <group id="3000">
                <function start="139" end="139" mask="00001100b">master</function>
                <function start="139" end="139" mask="00110000b">nicht_aktiv</function>
                <function start="75" end="75" mask="11111111b">english_uk</function>
                <function start="21" end="21" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE HUD Distance Info (Part 1 of 3 - See KOMBI and KAFAS2)">
            <group id="3000">
                <function start="97" end="97" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="Changes Default Time settings to 24H">
            <group id="3004">
                <function start="8" end="8" mask="00010000b">24h</function>
            </group>
        </code>
        <code description="ENABLE HUD Entertainment Details. Part 2 of 2. See KOMBI">
            <group id="3000">
                <function start="21" end="21" comment="hud_entertainmentlist" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Additional Menu Item (Current Position) in Navigation System">
            <group id="3000">
                <function start="96" end="96" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Active Sound Design (M5 only). Part 2 of 2. See ASD">
            <group id="3000">
                <function start="57" end="57" comment="ASD_SOUND_OFF" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Active Sound Design Configuration Menu (M5 only). Part 2 of 2. See ASD">
            <group id="3000">
                <function start="105" end="105" comment="ASD_CONFIGURATION" mask="00000001b">aktiv</function>
                <function start="105" end="105" comment="ASD_SOUND_4" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Volume to be retained up to 50% rather than startup at 25%">
            <group id="3002">
                <function start="3" end="3" comment="VOL_MAX_ON" mask="11111111b">32</function>
            </group>
        </code>
        <code description="ENABLE 'Route Info' (Turn-by-Turn list of route)">
            <group id="3000">
                <function start="59" end="59" comment="NAVI_ROAD_PREVIEW" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="Removes Speedlock for Office/Service Messages">
            <group id="3000">
                <function start="35" end="35" comment="SERVICES_MESSAGES_SPEEDLOCK_CONDITION" mask="00111000b">00</function>
                <function start="56" end="56" comment="OFFICE_MESSAGES_SPEEDLOCK_CONDITION" mask="00001110b">00</function>
            </group>
        </code>
        <code description="ENABLE Owners Manual in Motion (Removes Speedlock)">
            <group id="3000">
                <function start="0" end="0" comment="SL06_IBA_1" mask="00100000b">nicht_aktiv</function>
                <function start="0" end="0" comment="SL07_IBA_2" mask="01000000b">nicht_aktiv</function>
                <function start="2" end="2" comment="SL21_IBA_3" mask="00010000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Album Cover Scale to Full-Size">
            <group id="3000">
                <function start="14" end="14" comment="ENT_MC_COVER_SCALE" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Bluetooth Device Pairing Speedlock">
            <group id="3000">
                <function start="1" end="1" comment="SL16_ADD_CEDEVICE" mask="10000000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Real-Time Traffic Info">
            <group id="3000">
                <function start="59" end="59" comment="NAVI_TRAFFIC_INFO_MAP" mask="00010000b">aktiv</function>
            </group>
            <group id="3002">
                <function start="23" end="23" comment="TI_CA_TMC" mask="00000100b">aktiv</function>
                <function start="24" end="24" comment="TI_VINFO" mask="00000010b">aktiv</function>
                <function start="23" end="23" comment="TI_TMC_REGIONAL" mask="00100000b">aktiv</function>
                <function start="23" end="23" comment="TI_FALLBACK_DISABLED" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Rear Camera Zoom -Trailer Mode-">
            <group id="3001">
                <function start="54" end="54" comment="MACRO_TRAILER_COUPLING" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Hold-Mode for Range Extender (I001/1012)">
            <group id="3000">
                <function start="12" end="12" comment="EV_MENU_AVAILABLE" mask="00001100b">rex</function>
            </group>
        </code>
        <code description="ENABLE Compass">
            <group id="3000">
                <function start="5" end="5" comment="COMPASS" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Eco Pro Display info in KOMBI">
            <group id="3000">
                <function start="6" end="6" comment="ECO_INFO_DISPLAY" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Bookmark of current playback position">
            <group id="3000">
                <function start="14" end="14" comment="ENT_MC_SONG_BOOKMARK" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Gracenote DB Installed AND Lookup via USB and PC">
            <group id="3000">
                <function start="14" end="14" comment="ENT_GRACENOTE_INSTALLED" mask="01000000b">aktiv</function>
                <function start="15" end="15" comment="ENT_GRACENOTE_USB" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Traffic Info Category">
            <group id="3000">
                <function start="16" end="16" comment="TRAFFIC_CATEGORIES" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Follow-Me-Home Key Setting">
            <group id="3000">
                <function start="26" end="26" comment="KEY_CONF_COMFORT_HOMELIGHT" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE NAVI Map Arrow View">
            <group id="3000">
                <function start="62" end="62" comment="NAVI_MAP_ARROWVIEW" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE NAVI SPLIT AND FULL Guiding Popup">
            <group id="3000">
                <function start="62" end="62" comment="NAVI_SPLIT_GUIDINGPOPUP" mask="00001000b">aktiv</function>
                <function start="62" end="62" comment="NAVI_FULL_GUIDINGPOPUP" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE IPhone Ringtone">
            <group id="3003">
                <function start="6" end="6" comment="INBAND_RINGING" mask="10000000b">01</function>
            </group>
        </code>
    </cafd>
    <cafd id="000000F9" name="HU_CICHB" author="SaNGRia">
        <code description="ENABLE Weather Band Radio">
            <group id="3002">
                <function start="2" end="2" comment="RADIO_WEATHERBAND" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="High-Beam Assistant – Auto-On">
            <group id="3000">
                <function start="0" end="0" comment="HIGH_BEAM_ASSISTANT" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Cell Phone Ringer (Iphone Only)">
            <group id="3003">
                <function start="6" end="6" comment="INBAND_RINGING" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Sports Displays. Part 1 of 2. See KOMBI">
            <group id="3000">
                <function start="47" end="47" comment="EFF_DYN_SPORT_CID" mask="00010000b">aktiv</function>
                <function start="61" end="61" comment="EFF_DYN_SPORT_UNIT" mask="00000100b">aktiv</function>
                <function start="7" end="7" comment="MACRO_FDS" mask="00110000b">popup_and_config</function>
            </group>
        </code>
        <code description="ENABLE Turn Signals in HUD. Part 1 of 2. See KOMBI">
            <group id="3000">
                <function start="22" end="22" comment="HUD_TURNSIGNAL" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Video in Motion">
            <group id="3000">
                <function start="8" end="8" comment="VIDEO_NUR_MIT_HANDBREMSE" mask="01000000b">nicht_aktiv</function>
                <function start="23" end="23" comment="SPEEDLOCK_X_KMH_MIN" mask="11111111b">FF</function>
                <function start="24" end="24" comment="SPEEDLOCK_X_KMH_MAX" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Full Text Lines in Office While Driving">
            <group id="3003">
                <function start="19" end="19" comment="PIM_DRIVING_TEXT_LENGTH" mask="00000111b">whole_text</function>
            </group>
        </code>
        <code description="DISABLE Audible Chirp/Beep When Locking Car">
            <group id="3000">
                <function start="8" end="8" comment="ACOUSTICAL_LOCK_CONFIRM" mask="00100000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Audible Chirp/Beep When Locking Car">
            <group id="3000">
                <function start="8" end="8" comment="ACOUSTICAL_LOCK_CONFIRM" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="Add Temperature and PSI to tire monitor screen">
            <group id="3001">
                <function start="20" end="20" comment="RDC_SAFETY" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Legal Disclaimers">
            <group id="3001">
                <function start="27" end="27" comment="LEGAL_DISCLAIMER_TIME" mask="11111111b">kein_ld</function>
                <function start="28" end="28" comment="MACRO_CAM_LEGALDISCLAIMER" mask="11111111b">kein_ld</function>
                <function start="29" end="29" comment="MACRO_NVICAM_LDISCLAIMER" mask="11111111b">kein_ld</function>
            </group>
        </code>
        <code description="ENABLE volume to be retained up to 100% rather than startup at 25%">
            <group id="3002">
                <function start="23" end="23" comment="VOL_MAX_ON" mask="11111111b">32</function>
            </group>
        </code>
        <code description="ENABLE Real-Time Traffic Info">
            <group id="3000">
                <function start="6" end="6" comment="NAVI_TRAFFIC_INFO_MAP" mask="00010000b">aktiv</function>
            </group>
            <group id="3002">
                <function start="13" end="13" comment="TI_CA_TMC" mask="00000010b">aktiv</function>
                <function start="14" end="14" comment="TI_VINFO" mask="00000100b">aktiv</function>
                <function start="13" end="13" comment="TI_TMC_REGIONAL" mask="00010000b">aktiv</function>
                <function start="13" end="13" comment="TI_FALLBACK_DISABLED" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Rear Camera Zoom -Trailer Mode-">
            <group id="3001">
                <function start="23" end="23" comment="MACRO_TRAILER_COUPLING" mask="00000001b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="000005B6" name="Combbox_Media" author="SaNGRia">
        <code description="ENABLE Iphone Ringtone over vehicle speakers">
            <group id="3001">
                <function start="1" end="1" comment="INBAND_RINGING" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="Max amount of messages/addresses stored in vehicle, max 50 (HU_CIC only)">
            <group id="3006">
                <function start="1" end="1" comment="MY_INFO_SUPPORTED_POIS" mask="00111111b">wert_50</function>
            </group>
        </code>
        <code description="ENABLE Basic Voice Recognition">
            <group id="3000">
                <function start="3" end="3" comment="SVS_EIN_AUS" mask="00000100b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000069" name="KOMBI" author="SaNGRia" series="F010,F015">
        <code description="ENABLE Sports Displays (ft lb and hp). Part 2 of 2. See HU_NBT">
            <group id="3008">
                <function start="8" end="8" mask="11110000b">lb_ft</function>
                <function start="9" end="9" mask="00001111b">PS</function>
            </group>
        </code>
        <code description="ENABLE HUD Turnsignal. Part 2 of 2. See HU_NBT (Excludes 6WB)">
            <group id="3008">
                <function start="5" end="5" mask="00000001b">aktiv</function>
            </group>
            <group id="3000">
                <function start="42" end="42" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE 1st fuel warning at 50 miles">
            <group id="3000">
                <function start="49" end="49" mask="11111111b">inaktiv</function>
            </group>
        </code>
        <code description="ENABLE Digital Speed in MPH (New BC Option)">
            <group id="3000">
                <function start="1" end="1" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Efficient Dynamics Graph Direction (Left to Right)">
            <group id="3003">
                <function start="3" end="3" comment="On the Left" mask="00100000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Efficient Dynamics Graph Direction (Right to Left)">
            <group id="3003">
                <function start="3" end="3" comment="On the Right" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Daytime Instrument Cluster at Night (Stays White)">
            <group id="3007">
                <function start="10" end="10" comment="Does not work on LCI's" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Nighttime Instrument Cluster at Day (Stays Orange)">
            <group id="3007">
                <function start="11" end="11" comment="Does not work on LCI's" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Orange Decorative Lines on Instrument Cluster">
            <group id="3000">
                <function start="41" end="41" mask="00000010b">orange</function>
            </group>
        </code>
        <code description="ENABLE Grey Decorative Lines on Instrument Cluster">
            <group id="3000">
                <function start="41" end="41" mask="00000010b">grau</function>
            </group>
        </code>
        <code description="DISABLE Trip Computer Auto Reset">
            <group id="3000">
                <function start="44" end="44" comment="BC_AUTORESET_ZEIT" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Trip Computer Auto Reset (0 Hours)">
            <group id="3000">
                <function start="44" end="44" comment="BC_AUTORESET_ZEIT" mask="11111111b">00</function>
            </group>
        </code>
        <code description="ENABLE HUD Do Not Pass/Pass with care. Part 1 of 2. See KAFAS">
            <group id="3000">
                <function start="13" end="13" comment="SPEED_LIMIT_GENERATION" mask="00110000b">sli_gen_2_npi</function>
                <function start="45" end="45" comment="HUD_NPI_ENABLE" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE HUD Distance Info (Part 2 of 3. See HU_NBT and KAFAS2)">
            <group id="3000">
                <function start="1" end="1" mask="00000001b">aktiv</function>
            </group>
            <group id="3008">
                <function start="6" end="6" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="Activate LIM Function in North American Cars (Part 1 of 2. See ICMQL)">
            <group id="3003">
                <function start="3" end="3" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE HUD Entertainment Details. Part 1 of 2. See HU_NBT">
            <group id="3000">
                <function start="41" end="41" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE HUD Telephone Details">
            <group id="3000">
                <function start="41" end="41" mask="00010000b">aktiv</function>
                <function start="41" end="41" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE GPS Sync For Clock">
            <group id="3000">
                <function start="1" end="1" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE RED/WHITE Navigation Graphics in the Instrument Cluster">
            <group id="3000">
                <function start="40" end="40" mask="00100000b">neue_farbtabelle</function>
            </group>
        </code>
        <code description="ENABLE ALL WHITE Change of the Navigation Graphics in the Instrument Cluster">
            <group id="3000">
                <function start="40" end="40" mask="00100000b">alte_farbtabelle</function>
            </group>
        </code>
        <code description="DISABLE Auto Start Stop notification in Cluster">
            <group id="3000">
                <function start="41" end="41" mask="10000000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Auto Start Stop notification in Cluster">
            <group id="3000">
                <function start="41" end="41" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Night Vision with Background Pedestrian Detection. Part 1 of 2. See NIVI">
            <group id="3003">
                <function start="4" end="4" comment="FGS_NIVI_KI_ENABLE" mask="00000001b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="000009C8" name="KOMBI L7_MID" author="SaNGRia" series="F020,F030">
        <code description="Trip Computer Auto Reset (Never)">
            <group id="3000">
                <function start="44" end="44" comment="BC_AUTORESET_ZEIT" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="Trip Computer Auto Reset (0 Hours)">
            <group id="3000">
                <function start="44" end="44" comment="BC_AUTORESET_ZEIT" mask="11111111b">00</function>
            </group>
        </code>
        <code description="DISABLE Digital Speed Display in Cluster">
            <group id="3000">
                <function start="1" end="1" comment="BC_DIGITAL_V" mask="00000010b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Digital Speed Display in Cluster">
            <group id="3000">
                <function start="1" end="1" comment="BC_DIGITAL_V" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Speed Correction">
            <group id="3000">
                <function start="1" end="1" mask="01000000b">Aktiv</function>
            </group>
        </code>
        <code description="DISABLE Speed Correction">
            <group id="3000">
                <function start="1" end="1" mask="01000000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Auto Start Stop notificaiton in Cluster">
            <group id="3003">
                <function start="6" end="6" mask="00001000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Day White Instrument Cluster at night">
            <group id="3007">
                <function start="10" end="10" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE LIM Function. Part 1 of 2. See ICM">
            <group id="3003">
                <function start="3" end="3" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="Changes M3/M4 Instrument Cluster Startup Logo to GTS">
            <group id="3000">
                <function start="0" end="0" mask="11110000b">0C</function>
            </group>
        </code>
        <code description="ENABLE Night Vision with Background Pedestrian Detection. Part 1 of 2. See NIVI">
            <group id="3003">
                <function start="7" end="7" comment="FGS_NIVI_KI_ENABLE" mask="00001000b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001060" name="KOMBI FPK_I12" author="SaNGRia" series="I001">
        <code description="ENABLE HUD Turnsignal Blinkers (NOT with 6WB Digital Cluster). Part 1 of 2. See HU_NBT">
            <group id="3008">
                <function start="5" end="5" comment="HUD_PIA_BLINKER" mask="00000001b">aktiv</function>
            </group>
            <group id="3003">
                <function start="11" end="11" comment="HUD_BLINKER_ENABLE" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Night Vision with Background Pedestrian Detection. Part 1 of 2. See NIVI">
            <group id="3003">
                <function start="4" end="4" comment="FGS_NIVI_KI_ENABLE" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Range Extender Activation Battery Capacity (12%)">
            <group id="3000">
                <function start="46" end="46" comment="SOC_HOLD_POS" mask="11111111b">18</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000141F" name="KOMBI_I01_F56" author="SaNGRia" series="I001">
        <code description="ENABLE HUD Turnsignal Blinkers (NOT with 6WB Digital Cluster). Part 1 of 2. See HU_NBT">
            <group id="3008">
                <function start="7" end="7" comment="HUD_PIA_BLINKER" mask="00000001b">aktiv</function>
            </group>
            <group id="3003">
                <function start="4" end="4" comment="HUD_BLINKER_ENABLE" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Night Vision with Background Pedestrian Detection. Part 1 of 2. See NIVI">
            <group id="3000">
                <function start="43" end="43" comment="FGS_NIVI_KI_ENABLE" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="Increase Computer-limited fuel tank capacity of REX to full 2.4 US Gal (NOT 17-18)">
            <group id="3005">
                <function start="7" end="7" comment="TNK_VOLL_ANZEIGE" mask="11111111b">8_liter</function>
                <function start="8" end="17" comment="TNK_LITER_RECHTS" mask="11111111b">mcv_rex_liter_kl_rechts</function>
                <function start="28" end="47" comment="TNK_OHM_RECHTS" mask="11111111b">mcv_rex_ohm_kl_rechts_us</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000004C" name="NIVI2" author="SaNGRia" series="F010">
        <code description="ENABLE Night Vision with Background Pedestrian Detection. Part 1 of 2. See KOMBI">
            <group id="3000">
                <function start="20" end="20" comment="CC_Messages" mask="00000001b">ACTIVE_NV2P_BD</function>
            </group>
            <group id="3240">
                <function start="21" end="21" comment="DTC_ENABLE_13" mask="11111111b">FF</function>
            </group>
            <group id="3250">
                <function start="0" end="0" comment="USE_ACUTE_WARNING" mask="00010000b">AW_ON</function>
                <function start="0" end="0" comment="USE_ACUTE_SOUND" mask="10000000b">AW_ON</function>
            </group>
            <group id="3252">
                <function start="0" end="0" comment="R1_ACTIVE" mask="00000001b">AW_ON</function>
            </group>
            <group id="3253">
                <function start="50" end="50" comment="PED_DET_IN_BACKGROUND" mask="00100001b">ON</function>
            </group>
        </code>
        <code description="ENABLE Night Vision Pedestrian Detection at ANY speed (Default is at 8 mph)">
            <group id="3252">
                <function start="89" end="89" comment="BD_MINIMUM_SPEED" mask="00111111b">00</function>
            </group>
        </code>
        <code description="ENABLE Night Vision Camera on – Standby (Default when dark outside)">
            <group id="3000">
                <function start="23" end="23" comment="Light_Sensor" mask="00110000b">ON_WITH_PWR_ON</function>
            </group>
        </code>
    </cafd>
    <cafd id="000013D8" name="ICMQL" author="SaNGRia" series="F015">
        <code description="ENABLE Blind Spot Detection at 20km/h (13mph)">
            <group id="3000">
                <function start="190" end="190" mask="00111111b">20 kmh</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at ONE (1) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_1</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at TWO (2) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_2</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at THREE (3) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_3</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at FOUR (4) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_4</function>
            </group>
        </code>
        <code description="F15 - ENABLE Comfort Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode1 - Comfort" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE Comfort+ Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode2 - Comfort+" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE Unknown1 Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode3 - Unknown1" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE Sport Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode4 - Sport" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE Sport+ Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode5 - Sport+" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE Unknown2 Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode6 - Unknown2" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE EcoPro Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode7 - EcoPro" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="F15 - ENABLE Edrive Drive Mode">
            <group id="300A">
                <function start="62" end="62" comment="feshasmode8 - Edrive" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Remember Comfort+ Drive Mode When Shutdown - F15">
            <group id="300A">
                <function start="63" end="63" comment="fesallowmode2lastfunction - Comfort+" mask="00000100b">aktiv</function>
                <function start="79" end="79" comment="feslastfunctioninterval - Prevent Reset" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Remember Sport Drive Mode When Shutdown - F15">
            <group id="300A">
                <function start="63" end="63" comment="fesallowmode4lastfunction - Sport" mask="00001000b">aktiv</function>
                <function start="79" end="79" comment="feslastfunctioninterval - Prevent Reset" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Remember Sport+ Drive Mode When Shutdown - F15">
            <group id="300A">
                <function start="63" end="63" comment="fesallowmode7lastfunction - EcoPro" mask="00010000b">aktiv</function>
                <function start="79" end="79" comment="feslastfunctioninterval - Prevent Reset" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Remember Edrive Drive Mode When Shutdown - F15">
            <group id="300A">
                <function start="63" end="63" comment="fesallowmode8lastfunction - Edrive" mask="00100000b">aktiv</function>
                <function start="79" end="79" comment="feslastfunctioninterval - Prevent Reset" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Increased Traffic Jam Assistant (TJA) Max Speed - MPH">
            <group id="3000">
                <function start="191" end="191" comment="C_QalcgRel_v_Tacho_aktiv_mph" mask="00111111b">3F</function>
            </group>
        </code>
        <code description="ENABLE Increased Traffic Jam Assistant (TJA) Max Speed - KMH">
            <group id="3000">
                <function start="208" end="208" comment="C_QalcgRel_v_Tacho_aktiv_kmh" mask="11111111b">63</function>
            </group>
        </code>
        <code description="ENABLE Traffic Jam Assistant (TJA) on ALL ROADS">
            <group id="3000">
                <function start="97" end="97" comment="C_STA_Einschraenkung" mask="11100000b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000067B" name="ICMQL" author="SaNGRia" series="F010">
        <code description="Activate LIM Function in North American Cars (Part 2 of 2. See KOMBI)">
            <group id="3000">
                <function start="173" end="173" mask="00000001b">aktiv</function>
                <function start="197" end="197" mask="11100000b">zugelassen</function>
            </group>
        </code>
        <code description="ENABLE Blindspot Detection at 20kmh (13 mph)">
            <group id="3000">
                <function start="190" end="190" mask="00111111b">20 kmh</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at ONE (1) block">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_1</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at TWO (2) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_2</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at THREE (3) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_3</function>
            </group>
        </code>
        <code description="ENABLE default ACC distance at FOUR (4) blocks">
            <group id="3000">
                <function start="184" end="184" mask="00000111b">Stufe_4</function>
            </group>
        </code>
        <code description="ENABLE Default ECO PRO drive mode startup">
            <group id="3000">
                <function start="36" end="36" comment="ICMKOD_B_InitEco" mask="00001000b">verbaut</function>
            </group>
        </code>
        <code description="ENABLE Default COMFORT drive mode startup">
            <group id="3000">
                <function start="36" end="36" comment="ICMKOD_B_InitEco" mask="00001000b">nicht_verbaut</function>
            </group>
        </code>
        <code description="ENABLE Increased Traffic Jam Assistant (TJA) Max Speed - MPH">
            <group id="3000">
                <function start="191" end="191" comment="C_QalcgRel_v_Tacho_aktiv_mph" mask="00111111b">3F</function>
            </group>
        </code>
        <code description="ENABLE Increased Traffic Jam Assistant (TJA) Max Speed - KMH">
            <group id="3000">
                <function start="208" end="208" comment="C_QalcgRel_v_Tacho_aktiv_kmh" mask="11111111b">63</function>
            </group>
        </code>
        <code description="ENABLE Traffic Jam Assistant (TJA) on ALL ROADS">
            <group id="3000">
                <function start="97" end="97" comment="C_STA_Einschraenkung" mask="11100000b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000052" name="ICMQL" author="SaNGRia">
        <code description="ENABLE Blindspot Detection at 25kmh (15.5 mph)">
            <group id="3000">
                <function start="65" end="65" comment="Hc2_i_CPar_Aktiv_v_low" mask="11111111b">25 kmh</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000106D" name="FRM_03CT" author="SaNGRia" series="F010">
        <code description="ENABLE Open/Close windows and mirrors via keyFOB - CA. Part 1 of 2. See CAS (NA Cars)">
            <group id="3020">
                <function start="0" end="0" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Auto-Activate Hazard Warning System (Emergency Lights)">
            <group id="3050">
                <function start="2" end="2" comment="Sudden Stops at 70 km/h (~43 mph)" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Welcome Fog Lights - Soft LED">
            <group id="3050">
                <function start="29" end="29" mask="00001100b">soft_on_LED</function>
            </group>
        </code>
        <code description="ENABLE EU Brake Light Behavior (Blink)">
            <group id="3050">
                <function start="23" end="23" comment="Default = glow brighter and wider" mask="01110000b">02</function>
            </group>
        </code>
        <code description="ENABLE Increased Passenger Mirror Tilt (Curb View) in Reverse">
            <group id="3020">
                <function start="1" end="1" mask="11111111b">5A</function>
            </group>
        </code>
        <code description="ENABLE Fog Lights with High Beams">
            <group id="3050">
                <function start="16" end="16" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Front and Rear DRL (8TL)">
            <group id="3050">
                <function start="20" end="20" mask="00001110b">DRL_S</function>
            </group>
        </code>
        <code description="ENABLE Automatic High Beams Assistant (HBA)">
            <group id="3050">
                <function start="20" end="20" mask="00100000b">automatisch</function>
            </group>
        </code>
        <code description="ENABLE FRONT driver/passenger window Roll Up when doors opened (JBBFE for Rear)">
            <group id="3030">
                <function start="1" end="1" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="Easy Entry/Exit Steering Wheel and Driver Seat (Tilt First). Step 1 of 2. See SM">
            <group id="30A0">
                <function start="9" end="9" mask="10000000b">aktiv</function>
                <function start="10" end="10" mask="10000000b">aktiv</function>
                <function start="1" end="1" comment="Tilt Adjust 1st" mask="11000000b">02</function>
            </group>
        </code>
        <code description="Easy Entry/Exit Steering Wheel and Driver Seat (Longitudinal 1st). Step 1 of 2. See SM">
            <group id="30A0">
                <function start="9" end="9" mask="10000000b">aktiv</function>
                <function start="10" end="10" mask="10000000b">aktiv</function>
                <function start="1" end="1" comment="Tilt Adjust 1st" mask="11000000b">01</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000106D" name="FRM_03CT" author="SaNGRia" series="F025">
        <code description="F25 NGHB. Part 3 of 3. See LHM43/LHM44. Step 3 of PDF">
            <group id="3080">
                <function start="32" end="35" comment="LAMP_MAP_PARA_SATZ_09" mask="11111111b">00, 00, 00, 00</function>
                <function start="36" end="39" comment="LAMP_MAP_PARA_SATZ_10" mask="11111111b">00, 00, 00, 00</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000012F" name="FRM_O3CT" author="SaNGRia" series="F010">
        <code description="ENABLE Folding Mirrors/Window Rollup. Part 1 of 2. See CAS">
            <group id="3020">
                <function start="0" end="0" comment="ASP_BEIKLAPPEN_BEI_KOMFORTSCHLIESSEN" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Increased Passenger Mirror Tilt (Curb View) in Reverse">
            <group id="3020">
                <function start="1" end="1" comment="ASP_BORDSTEINAUTOMATIK_DELTA" mask="11111111b">5A</function>
            </group>
        </code>
        <code description="ENABLE Variable Light Distribution (VLD)">
            <group id="3400">
                <function start="2" end="2" comment="AHL2_ENABLE" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Auto-Activate Hazard Warning System (Emergency Lights)">
            <group id="3050">
                <function start="2" end="2" comment="Sudden Stops at 70 km/h (~43 mph)" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Welcome Fog Lights - Soft LED">
            <group id="3050">
                <function start="29" end="29" mask="00001100b">soft_on_LED</function>
            </group>
        </code>
        <code description="ENABLE EU Brake Light Behavior (Blink)">
            <group id="3050">
                <function start="23" end="23" comment="Default = glow brighter and wider" mask="01110000b">02</function>
            </group>
        </code>
        <code description="ENABLE Fog Lights with High Beams">
            <group id="3050">
                <function start="16" end="16" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Front and Rear DRL (8TL)">
            <group id="3050">
                <function start="20" end="20" mask="00001110b">DRL_S</function>
            </group>
        </code>
        <code description="ENABLE Automatic High Beams Assistant (HBA)">
            <group id="3050">
                <function start="20" end="20" mask="00100000b">automatisch</function>
            </group>
        </code>
        <code description="ENABLE FRONT driver/passenger window Roll Up when doors opened (JBBFE for Rear)">
            <group id="3030">
                <function start="1" end="1" mask="00000100b">00</function>
            </group>
        </code>
        <code description="Easy Entry/Exit Steering Wheel and Driver Seat (Tilt First). Step 1 of 2. See SM">
            <group id="30A0">
                <function start="9" end="9" mask="10000000b">aktiv</function>
                <function start="10" end="10" mask="10000000b">aktiv</function>
                <function start="1" end="1" comment="Tilt Adjust 1st" mask="11000000b">02</function>
            </group>
        </code>
        <code description="Easy Entry/Exit Steering Wheel and Driver Seat (Longitudinal 1st). Step 1 of 2. See SM">
            <group id="30A0">
                <function start="9" end="9" mask="10000000b">aktiv</function>
                <function start="10" end="10" mask="10000000b">aktiv</function>
                <function start="1" end="1" comment="Longitude Adjust 1st" mask="11000000b">01</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000000F" name="CAS_04" author="SaNGRia" series="F010">
        <code description="DISABLE Auto Start Stop (ASS) by Default">
            <group id="3000">
                <function start="3" end="3" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Auto Start Stop (ASS) Memory - Shutdown Setting">
            <group id="3000">
                <function start="3" end="3" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Open/Close windows and mirrors via keyFOB - CA (NA Cars). Part 2 of 2. See FRM">
            <group id="3003">
                <function start="2" end="2" mask="00000001b">aktiv</function>
                <function start="2" end="2" mask="00000010b">aktiv</function>
                <function start="2" end="2" mask="00000100b">aktiv</function>
                <function start="2" end="2" mask="00001000b">aktiv</function>
                <function start="2" end="2" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="Removes Initiation Delay for Mirrors/Windows">
            <group id="3003">
                <function start="12" end="12" mask="11111111b">00</function>
            </group>
        </code>
        <code description="ENABLE Auto Unlock doors when engine stopped (Requires Auto-Lock)">
            <group id="3002">
                <function start="1" end="1" comment="Single pull to open" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Auto Unlock doors when engine stopped (Requires Auto-Lock)">
            <group id="3002">
                <function start="1" end="1" comment="Single pull to open" mask="10000000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Horn Lock Confirmation while engine running">
            <group id="3002">
                <function start="0" end="0" comment="CLM_HORN_AT_SECURE" mask="00100000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Horn Lock Confirmation while engine running">
            <group id="3002">
                <function start="0" end="0" comment="CLM_HORN_AT_SECURE" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Follow Me Home Lighting with Short Press of Panic Button">
            <group id="3002">
                <function start="1" end="1" comment="REMOTE_KEY_SPECIAL_FCT" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Follow Me Home Lighting with Short Press of Panic Button">
            <group id="3002">
                <function start="1" end="1" comment="REMOTE_KEY_SPECIAL_FCT" mask="00000010b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Engine Start without Brake Pedal (Press Start Twice with Second Hold)">
            <group id="3000">
                <function start="1" end="1" comment="TC_STARTLOCK_BRAKE" mask="00000001b">nicht_aktiv</function>
                <function start="1" end="1" comment="TC_STARTLOCK_DRIVINGREADINESS" mask="00010000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Engine Start without Brake Pedal (Press Start Twice with Second Hold)">
            <group id="3000">
                <function start="1" end="1" comment="TC_STARTLOCK_BRAKE" mask="00000001b">aktiv</function>
                <function start="1" end="1" comment="TC_STARTLOCK_DRIVINGREADINESS" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE  Radio and Nav Off when drivers door opened">
            <group id="3000">
                <function start="2" end="2" comment="TC_LOGIC_KLR_OFF_DOOR" mask="00000001b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000C18" name="DSC_Premium" author="SaNGRia" series="F010">
        <code description="ENABLE Auto-Parking Brake Release (Only 2010-2012 cars). Part 1 of 2. See EMF">
            <group id="3000">
                <function start="27" end="27" comment="Funktion_AutomaticDriveawayRelease_aktiv" mask="00100000b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000029B" name="EMF_03TRW" author="SaNGRia" series="F010">
        <code description="ENABLE Auto-Parking Brake Release (Only 2010-2012 cars). Part 2 of 2. See DSC">
            <group id="3000">
                <function start="0" end="0" comment="ADR_ein" mask="00001000b">ADR_Ein</function>
            </group>
        </code>
    </cafd>
    <cafd id="000000B5" name="CFAS-PLX_1" author="SaNGRia" series="F010,F015,F030,F80">
        <code description="Time Period Seats will Remember heating/cooling/massage settings (0 minutes)">
            <group id="3000">
                <function start="4" end="4" comment="0 minutes" mask="00000011b">00</function>
            </group>
        </code>
        <code description="Time Period Seats will Remember heating/cooling/massage settings (15 minutes)">
            <group id="3000">
                <function start="4" end="4" comment="15 minutes" mask="00000011b">01</function>
            </group>
        </code>
        <code description="Time Period Seats will Remember heating/cooling/massage settings (24 hours)">
            <group id="3000">
                <function start="4" end="4" comment="24 hours" mask="00000011b">02</function>
            </group>
        </code>
        <code description="Time Period Seats will Remember heating/cooling/massage settings (Infinity)">
            <group id="3000">
                <function start="4" end="4" comment="Infinity" mask="00000011b">03</function>
            </group>
        </code>
        <code description="Easy Entry/Exit Steering Wheel and Driver Seat. Step 1 of 2. See FRM for F10">
            <group id="3000">
                <function start="0" end="0" mask="00011100b">Modus_FA_SLV</function>
            </group>
            <group id="3012">
                <function start="0" end="1" mask="11111111b">00, 28</function>
                <function start="4" end="5" mask="11111111b">00, 32</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000033D" name="SZL_LWS_03" author="SaNGRia" series="F010">
        <code description="ENABLE Steering Paddle Shifters">
            <group id="3000">
                <function start="0" end="0" comment="Lenkrad_Schaltpaddles" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Steering Paddle Shifters">
            <group id="3000">
                <function start="0" end="0" comment="Lenkrad_Schaltpaddles" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000014" name="JBBFE" author="SaNGRia" series="F010">
        <code description="ENABLE REAR driver/passenger window Roll Up when doors opened FRM for Front)">
            <group id="3070">
                <function start="0" end="0" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Reduced Rain HeadLight Sensor Sensitivity (Insensitive)">
            <group id="3530">
                <function start="5" end="5" mask="00000111b">unempfindlich</function>
                <function start="5" end="5" mask="00111000b">unempfindlich</function>
            </group>
        </code>
        <code description="Adjust Rear and Side Mirror Dimming for Dark Windows">
            <group id="3080">
                <function start="1" end="1" mask="00000110b">Dunkel</function>
                <function start="20" end="20" mask="11111100b">39</function>
                <function start="28" end="28" mask="11111100b">39</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000018" name="JBBF_E3_PDC" author="SaNGRia" series="F010">
        <code description="ENABLE Top/Rear Camera at All Speeds. Part 1 of 2. See TRSVC for Side">
            <group id="3009">
                <function start="15" end="15" comment="max speed to disable top camera view" mask="11111111b">FF</function>
                <function start="16" end="16" comment="max speed to disable rear camera view" mask="11111111b">FF</function>
                <function start="17" end="17" comment="max distance to disable top camera view" mask="11111111b">FF</function>
                <function start="18" end="18" comment="max distance to disable rear camera view" mask="11111111b">FF</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000223" name="TRSVC" author="SaNGRia" series="F010,F030,F080">
        <code description="Side Camera at All Speeds. Part 1 of 2. See PDC for Top/Rear">
            <group id="3000">
                <function start="114" end="114" comment="Maximum speed side view can activate" mask="11111111b">FF</function>
                <function start="115" end="115" comment="Auto-deactivate side view speed" mask="11111111b">FF</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000909" name="ACSM_4C" author="SaNGRia" series="F010,F015">
        <code description="DISABLE Seat Belt Instrument Cluster Status (Passenger)">
            <group id="3000">
                <function start="15" end="15" mask="00010000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Instrument Cluster Status (Driver)">
            <group id="3000">
                <function start="15" end="15" mask="00001000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder Chime (Driver)">
            <group id="3000">
                <function start="15" end="15" mask="00000010b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder Chime(Passenger)">
            <group id="3000">
                <function start="15" end="15" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Initial Belt Warning Chime (845 Acoustic Belt Warning)">
            <group id="3000">
                <function start="15" end="15" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder PreWarning Chime (Driver)">
            <group id="3000">
                <function start="16" end="16" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder PreWarning Chime (Passenger)">
            <group id="3000">
                <function start="16" end="16" mask="00000010b">nicht_aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000009C" name="ACSM_3" author="SaNGRia" series="F010">
        <code description="DISABLE Seat Belt Instrument Cluster Status (Passenger)">
            <group id="3000">
                <function start="11" end="11" comment="Gurtzustandsanzeige_Beifahrer_GWF_GZA_BF" mask="00010000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Instrument Cluster Status (Driver)">
            <group id="3000">
                <function start="11" end="11" comment="Gurtzustandsanzeige_Fahrer_GWF_GZA_FA" mask="00001000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder Chime (Driver)">
            <group id="3000">
                <function start="11" end="11" comment="SBR_FA_GWF_SBR_FA" mask="00000010b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder Chime Passenger)">
            <group id="3000">
                <function start="11" end="11" comment="SBR_BF_GWF_SBR_BF" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Initial Belt Warning Chime (845 Acoustic Belt Warning)">
            <group id="3000">
                <function start="11" end="11" comment="Initialwarnung_GWF_IW" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="000011AB" name="ACSM_4i" author="SaNGRia" series="I001">
        <code description="DISABLE Seat Belt Reminder (Driver) - Old Firmware">
            <group id="3001">
                <function start="1" end="1" comment="SeatBeltReminder_Fahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder (Passenger) - Old Firmware">
            <group id="3001">
                <function start="2" end="2" comment="SeatBeltReminder_Beifahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Disconnected Reminder Sound (Driver) - Old Firmware">
            <group id="3001">
                <function start="3" end="3" comment="SBR_PreWarning_Fahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Disconnected Reminder Sound (Passenger) - Old Firmware">
            <group id="3001">
                <function start="4" end="4" comment="SBR_PreWarning_Beifahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Initial Belt Warning Gong - Old Firmware">
            <group id="3001">
                <function start="0" end="0" comment="Initialwarnung" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000F9B" name="ASD01" author="SaNGRia" series="F010,F080">
        <code description="DISABLE Active Sound Design (M5 only). Part 1 of 2. See HU_NBT">
            <group id="3000">
                <function start="0" end="0" comment="Model Range" mask="11111111b">0D</function>
                <function start="1" end="1" comment="Model Range" mask="11111111b">08</function>
            </group>
        </code>
    </cafd>
    <cafd id="000024C3" name="FLE_02" author="SaNGRia" series="F015">
        <code description="F15 - Turn off Front DRL Headlight dim (Stay 100 Percent). Do Both FLEs">
            <group id="3004">
                <function start="10" end="19" mask="11111111b">01, 01, 0A, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="20" end="29" mask="11111111b">01, 01, 0A, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="30" end="39" mask="11111111b">01, 01, 0A, 01, 01, 01, 01, 01, 01, 0B</function>
            </group>
        </code>
        <code description="F15 - Turn off Amber Sidemarker on Headlights">
            <group id="3006">
                <function start="41" end="41" mask="11110000b">00</function>
                <function start="49" end="49" mask="11111111b">00</function>
            </group>
        </code>
        <code description="F15 (After July 1 2015) - NGHB. Apply to Both FLEs. Step 2 of PDF">
            <group id="3003">
                <function start="20" end="29" comment="Stadt_V_Idx" mask="11111111b">04, 01, 01, 01, 02, 03, 01, 01, 05, 01</function>
                <function start="30" end="39" comment="SAE_Idx" mask="11111111b">04, 01, 01, 01, 02, 03, 01, 01, 01, 01</function>
                <function start="120" end="129" comment="H_plus4_Idx" mask="11111111b">04, 01, 01, 01, 02, 03, 01, 01, 01, 01</function>
                <function start="130" end="139" comment="Blendfreies_Fernlicht_Idx" mask="11111111b">01, 06, 01, 01, 06, 06, 01, 01, 01, 01</function>
                <function start="140" end="149" comment="Volles_Fernlicht_" mask="11111111b">07, 07, 01, 01, 07, 07, 07, 01, 01, 01</function>
            </group>
            <group id="3004">
                <function start="0" end="9" comment="DRL_Idx" mask="11111111b">01, 01, 0A, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="10" end="19" comment="POLI1_Idx" mask="11111111b">01, 01, 0C, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="20" end="29" comment="POLI2_Idx" mask="11111111b">01, 01, 0C, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="30" end="39" comment="POLI3_Idx" mask="11111111b">01, 01, 0C, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="40" end="49" comment="PLI_Idx" mask="11111111b">01, 01, 0C, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="60" end="69" comment="WELL1_Idx" mask="11111111b">01, 01, 0E, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="70" end="79" comment="WELL2_Idx" mask="11111111b">01, 01, 0E, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="80" end="89" comment="WELL3_Idx" mask="11111111b">01, 0F, 01, 01, 01, 01, 01, 01, 01, 0B</function>
                <function start="90" end="99" comment="WELL4_Idx" mask="11111111b">01, 0F, 01, 01, 01, 01, 0F, 01, 01, 0B</function>
                <function start="100" end="109" comment="FMH_Idx" mask="11111111b">10, 01, 0E, 01, 10, 10, 01, 01, 01, 0B</function>
                <function start="110" end="119" comment="REMLI_Idx" mask="11111111b">10, 01, 0E, 01, 10, 10, 01, 01, 01, 0B</function>
                <function start="120" end="129" comment="HBBLINK_Idx" mask="11111111b">0F, 08, 0F, 01, 0F, 0F, 08, 01, 01, 0B</function>
                <function start="130" end="139" comment="DWABLINK_Idx" mask="11111111b">01, 01, 01, 01, 01, 01, 01, 0F, 01, 01</function>
                <function start="140" end="149" comment="PANICMODE_Idx" mask="11111111b">01, 01, 01, 01, 01, 01, 01, 01, 01, 01</function>
                <function start="150" end="159" comment="RAIDALARM_Idx" mask="11111111b">01, 08, 0F, 01, 01, 01, 08, 0F, 01, 11</function>
                <function start="160" end="169" comment="BLINKEN_Idx" mask="11111111b">01, 01, 01, 01, 01, 01, 01, 0F, 01, 11</function>
                <function start="180" end="189" comment="SIDEMRKLGT_Idx" mask="11111111b">01, 01, 01, 0F, 01, 01, 01, 01, 01, 01</function>
            </group>
            <group id="3000">
                <function start="4" end="4" comment="HlPrjLabel_HlType" mask="11110000b">0A</function>
            </group>
            <group id="3005">
                <function start="3" end="3" comment="LmmIdx00_ErrorImpact" mask="01000000b">00</function>
                <function start="11" end="11" comment="LmmIdx02_ErrorImpact" mask="01000000b">00</function>
                <function start="15" end="15" comment="LmmIdx03_ErrorImpact" mask="01000000b">00</function>
                <function start="16" end="16" comment="LmmIdx04_Intensity" mask="11111111b">00</function>
                <function start="17" end="17" comment="LmmIdx04_TimeOn" mask="11111111b">04</function>
                <function start="18" end="18" comment="LmmIdx04_TimeOff" mask="11111111b">04</function>
                <function start="19" end="19" comment="LmmIdx04_ErrorImpact" mask="01000000b">00</function>
                <function start="20" end="20" comment="LmmIdx05_Intensity" mask="11111111b">2E</function>
                <function start="21" end="21" comment="LmmIdx05_TimeOn" mask="11111111b">04</function>
                <function start="22" end="22" comment="LmmIdx05_TimeOff" mask="11111111b">04</function>
                <function start="23" end="23" comment="LmmIdx05_ErrorImpact" mask="01000000b">00</function>
                <function start="24" end="24" comment="LmmIdx06_Intensity" mask="11111111b">64</function>
                <function start="25" end="25" comment="LmmIdx06_TimeOn" mask="11111111b">04</function>
                <function start="27" end="27" comment="LmmIdx06_ErrorImpact" mask="01000000b">00</function>
                <function start="31" end="31" comment="LmmIdx07_Priority" mask="00001111b">01</function>
                <function start="31" end="31" comment="LmmIdx07_ErrorImpact" mask="01000000b">00</function>
                <function start="36" end="36" comment="LmmIdx09_Intensity" mask="11111111b">2E</function>
                <function start="39" end="39" comment="LmmIdx09_Priority" mask="00001111b">03</function>
                <function start="39" end="39" comment="LmmIdx09_ErrorImpact" mask="01000000b">00</function>
                <function start="40" end="40" comment="LmmIdx10_Intensity" mask="11111111b">64</function>
                <function start="43" end="43" comment="LmmIdx10_Priority" mask="00001111b">02</function>
                <function start="44" end="44" comment="LmmIdx11_Intensity" mask="11111111b">64</function>
                <function start="47" end="47" comment="LmmIdx11_Priority" mask="00001111b">03</function>
                <function start="47" end="47" comment="LmmIdx11_ErrorImpact" mask="01000000b">00</function>
                <function start="48" end="48" comment="LmmIdx12_Intensity" mask="11111111b">29</function>
                <function start="51" end="51" comment="LmmIdx12_Priority" mask="00001111b">03</function>
                <function start="51" end="51" comment="LmmIdx12_ErrorImpact" mask="01000000b">01</function>
                <function start="53" end="53" comment="LmmIdx13_TimeOn" mask="11111111b">08</function>
                <function start="54" end="54" comment="LmmIdx13_TimeOff" mask="11111111b">19</function>
                <function start="55" end="55" comment="LmmIdx13_Priority" mask="00001111b">01</function>
                <function start="56" end="56" comment="LmmIdx14_Intensity" mask="11111111b">29</function>
                <function start="57" end="57" comment="LmmIdx14_TimeOn" mask="11111111b">00</function>
                <function start="58" end="58" comment="LmmIdx14_TimeOff" mask="11111111b">00</function>
                <function start="59" end="59" comment="LmmIdx14_Priority" mask="00001111b">04</function>
                <function start="59" end="59" comment="LmmIdx14_ErrorImpact" mask="01000000b">01</function>
                <function start="60" end="60" comment="LmmIdx15_Intensity" mask="11111111b">64</function>
                <function start="63" end="63" comment="LmmIdx15_Active" mask="10000000b">00</function>
                <function start="64" end="64" comment="LmmIdx16_Intensity" mask="11111111b">64</function>
                <function start="65" end="65" comment="LmmIdx16_TimeOn" mask="11111111b">04</function>
                <function start="66" end="66" comment="LmmIdx16_TimeOff" mask="11111111b">04</function>
                <function start="67" end="67" comment="LmmIdx16_Priority" mask="00001111b">0A</function>
                <function start="71" end="71" comment="LmmIdx17_Priority" mask="00001111b">01</function>
                <function start="71" end="71" comment="LmmIdx17_Active" mask="10000000b">01</function>
                <function start="72" end="72" comment="LmmIdx18_Intensity" mask="11111111b">5B</function>
                <function start="73" end="73" comment="LmmIdx18_TimeOn" mask="11111111b">04</function>
                <function start="74" end="74" comment="LmmIdx18_TimeOff" mask="11111111b">04</function>
                <function start="75" end="75" comment="LmmIdx18_Priority" mask="00001111b">01</function>
                <function start="134" end="134" comment="LmmReLut_LgtFct0" mask="00111111b">01</function>
                <function start="134" end="134" comment="LmmReLut_LogLmpLow0" mask="11000000b">01</function>
                <function start="135" end="135" comment="LmmReLut_Idx0" mask="11111100b">03</function>
                <function start="136" end="136" comment="LmmReLut_LgtFct1" mask="00111111b">02</function>
                <function start="136" end="136" comment="LmmReLut_LogLmpLow1" mask="11000000b">01</function>
                <function start="137" end="137" comment="LmmReLut_Idx1" mask="11111100b">03</function>
                <function start="138" end="138" comment="LmmReLut_LgtFct2" mask="00111111b">03</function>
                <function start="138" end="138" comment="LmmReLut_LogLmpLow2" mask="11000000b">01</function>
                <function start="139" end="139" comment="LmmReLut_Idx2" mask="11111100b">12</function>
                <function start="140" end="140" comment="LmmReLut_LgtFct3" mask="00111111b">0D</function>
                <function start="140" end="140" comment="LmmReLut_LogLmpLow3" mask="11000000b">01</function>
                <function start="141" end="141" comment="LmmReLut_Idx3" mask="11111100b">03</function>
                <function start="142" end="142" comment="LmmReLut_LgtFct4" mask="00111111b">0E</function>
                <function start="142" end="142" comment="LmmReLut_LogLmpLow4" mask="11000000b">01</function>
                <function start="143" end="143" comment="LmmReLut_Idx4" mask="11111100b">0F</function>
                <function start="144" end="144" comment="LmmReLut_LgtFct5" mask="00111111b">06</function>
                <function start="144" end="144" comment="LmmReLut_LogLmpLow5" mask="11000000b">01</function>
                <function start="145" end="145" comment="LmmReLut_LogLmpHigh5" mask="00000011b">01</function>
                <function start="145" end="145" comment="LmmReLut_Idx5" mask="11111100b">03</function>
                <function start="146" end="146" comment="LmmReLut_LgtFct6" mask="00111111b">07</function>
                <function start="146" end="146" comment="LmmReLut_LogLmpLow6" mask="11000000b">01</function>
                <function start="147" end="147" comment="LmmReLut_LogLmpHigh6" mask="00000011b">01</function>
                <function start="147" end="147" comment="LmmReLut_Idx6" mask="11111100b">03</function>
                <function start="148" end="148" comment="LmmReLut_LgtFct7" mask="00111111b">08</function>
                <function start="148" end="148" comment="LmmReLut_LogLmpLow7" mask="11000000b">01</function>
                <function start="149" end="149" comment="LmmReLut_LogLmpHigh7" mask="00000011b">01</function>
                <function start="149" end="149" comment="LmmReLut_Idx7" mask="11111100b">03</function>
                <function start="150" end="150" comment="LmmReLut_LgtFct8" mask="00111111b">09</function>
                <function start="150" end="150" comment="LmmReLut_LogLmpLow8" mask="11000000b">01</function>
                <function start="151" end="151" comment="LmmReLut_LogLmpHigh8" mask="00000011b">01</function>
                <function start="151" end="151" comment="LmmReLut_Idx8" mask="11111100b">03</function>
            </group>
        </code>
    </cafd>
    <cafd id="000024C3" name="FLE_02" author="SaNGRia" series="F030">
        <code description="F30LCI - HALO Brightness 100% with Non-Adaptive LED lowbeams. Do Both FLEs">
            <group id="3004">
                <function start="10" end="19" mask="11111111b">00, 00, 00, 00, 00, 00, 04, 00, 00, 00</function>
                <function start="20" end="29" mask="11111111b">00, 00, 00, 00, 00, 00, 04, 00, 00, 00</function>
                <function start="30" end="39" mask="11111111b">00, 00, 00, 00, 00, 00, 04, 00, 00, 00</function>
            </group>
        </code>
    </cafd>
    <cafd id="000010BA" name="LHM2" author="SaNGRia" series="F015">
        <code description="F15 (Before July 1 2015) - NGHB. Part 1 of 2. See LHM44">
            <group id="3000">
                <function start="0" end="6" comment="M1. Step 2 of PDF" mask="11111111b">FA, 64, 00, 00, 00, FA, 00</function>
                <function start="7" end="13" comment="M2. Step 2 of PDF" mask="11111111b">FA, 64, 00, 00, 00, FA, 00</function>
                <function start="14" end="20" comment="M3. Step 2 of PDF" mask="11111111b">FA, 00, 00, 00, 00, FA, 00</function>
                <function start="21" end="27" comment="M4. Step 2 of PDF" mask="11111111b">FA, 00, 00, 00, 00, C8, 00</function>
                <function start="91" end="97" comment="M14. Step 2 of PDF" mask="11111111b">FA, 00, FA, 00, 00, FA, 00</function>
                <function start="98" end="104" comment="M15. Step 2 of PDF" mask="11111111b">FA, FA, FA, 00, 00, FA, FA</function>
            </group>
        </code>
    </cafd>
    <cafd id="000010BA" name="LHM2" author="SaNGRia" series="F025">
        <code description="F25 NGHB. Part 1 of 3. See LHM44/FRM. Step 2 of PDF">
            <group id="3000">
                <function start="0" end="6" comment="M1" mask="11111111b">FA, 64, 00, 00, FA, FA, 00</function>
                <function start="7" end="13" comment="M2" mask="11111111b">FA, 64, 00, 00, FA, FA, 00</function>
                <function start="14" end="20" comment="M3" mask="11111111b">FA, 00, 00, 00, FA, FA, 00</function>
                <function start="21" end="27" comment="M4" mask="11111111b">FA, 00, 00, 00, C8, C8, 00</function>
                <function start="91" end="97" comment="M14" mask="11111111b">FA, 00, 00, FA, FA, FA, 00</function>
                <function start="98" end="104" comment="M15" mask="11111111b">FA, FA, 00, FA, FA, FA, FA</function>
            </group>
        </code>
    </cafd>
    <cafd id="000010BA" name="LHM2" author="SaNGRia" series="F030,F080">
        <code description="F3x and F8x NGHB. Step 1 of 3 - Driver side. See LHM44/FEM_Body">
            <group id="3000">
                <function start="0" end="6" comment="NGHB PDF Step 2" mask="11111111b">FA, 64, 00, 00, FA, FA, 00</function>
                <function start="7" end="13" comment="NGHB PDF Step 2" mask="11111111b">FA, 64, 00, 00, FA, FA, 00</function>
                <function start="14" end="20" comment="NGHB PDF Step 2" mask="11111111b">FA, 00, 00, 19, FA, FA, 00</function>
                <function start="21" end="27" comment="NGHB PDF Step 2" mask="11111111b">FA, 00, 00, 00, C8, C8, 00</function>
                <function start="91" end="97" comment="NGHB PDF Step 2" mask="11111111b">FA, 00, FA, 00, FA, FA, 00</function>
                <function start="98" end="104" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, FA, 00, FA, FA, FA</function>
            </group>
        </code>
    </cafd>
    <cafd id="000016BF" name="LHM2" author="SaNGRia" series="F015">
        <code description="F15 (Before July 1 2015) - NGHB. Part 2 of 2. See LHM43">
            <group id="3000">
                <function start="0" end="6" comment="M1. Step 2 of PDF" mask="11111111b">FA, FA, 00, 00, 00, FA, 00</function>
                <function start="7" end="13" comment="M2. Step 2 of PDF" mask="11111111b">FA, FA, 00, 00, 00, FA, 00</function>
                <function start="14" end="20" comment="M3. Step 2 of PDF" mask="11111111b">FA, BB, 00, 00, 00, FA, 00</function>
                <function start="21" end="27" comment="M4. Step 2 of PDF" mask="11111111b">FA, 00, 00, 00, 00, C8, 00</function>
                <function start="35" end="41" comment="M6. Step 2 of PDF" mask="11111111b">FA, FA, 00, 00, 00, FA, 00</function>
                <function start="42" end="48" comment="M7. Step 2 of PDF" mask="11111111b">FA, FA, 00, 00, 00, FA, 00</function>
                <function start="49" end="55" comment="M8. Step 2 of PDF" mask="11111111b">FA, FA, 00, 00, 00, FA, 00</function>
                <function start="56" end="62" comment="M9. Step 2 of PDF" mask="11111111b">FA, FA, 00, 00, 00, FA, 00</function>
                <function start="91" end="97" comment="M14. Step 2 of PDF" mask="11111111b">FA, FA, FA, 00, 00, FA, 00</function>
                <function start="98" end="104" comment="M15. Step 2 of PDF" mask="11111111b">FA, FA, FA, 00, 00, FA, FA</function>
            </group>
        </code>
    </cafd>
    <cafd id="000016BF" name="LHM2" author="SaNGRia" series="F025">
        <code description="F25 NGHB. Part 2 of 3. See LHM43/FRM. Step 2 of PDF">
            <group id="3000">
                <function start="0" end="6" comment="M1" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="7" end="13" comment="M2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="14" end="20" comment="M3" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="21" end="27" comment="M4" mask="11111111b">FA, 00, 00, 00, C8, C8, 00</function>
                <function start="35" end="41" comment="M6" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="42" end="48" comment="M7" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="49" end="55" comment="M8" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="56" end="62" comment="M9" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="91" end="97" comment="M14" mask="11111111b">FA, FA, 00, FA, FA, FA, 00</function>
                <function start="98" end="104" comment="M15" mask="11111111b">FA, FA, 00, FA, FA, FA, FA</function>
            </group>
        </code>
    </cafd>
    <cafd id="000016BF" name="LHM2" author="SaNGRia" series="F030,F080">
        <code description="F3x and F8x NGHB. Step 2 of 3- Passenger side. See LHM43/FEM_Body">
            <group id="3000">
                <function start="0" end="6" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="7" end="13" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="14" end="20" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 19, FA, FA, 00</function>
                <function start="21" end="27" comment="NGHB PDF Step 2" mask="11111111b">FA, 00, 00, 00, C8, C8, 00</function>
                <function start="35" end="41" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="42" end="48" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="49" end="55" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="56" end="62" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, 00, 00, FA, FA, 00</function>
                <function start="91" end="97" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, FA, 00, FA, FA, 00</function>
                <function start="98" end="104" comment="NGHB PDF Step 2" mask="11111111b">FA, FA, FA, 00, FA, FA, FA</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001082" name="TMS_03" author="SaNGRia" series="F010">
        <code description="Turn OFF Amber sidemarker lights. Part 1 of 2. See TMS42. (F10 LCI Xenon)">
            <group id="3005">
                <function start="16" end="31" comment="Standlicht Modus 1" mask="11111111b">F10_524_ECE</function>
                <function start="32" end="47" comment="Standlicht Modus 2" mask="11111111b">F10_524_ECE</function>
                <function start="48" end="63" comment="Standlicht Modus 3" mask="11111111b">F10_524_ECE</function>
                <function start="80" end="95" comment="Welcome Light 1" mask="11111111b">F10_524_ECE</function>
                <function start="144" end="159" comment="Follow Me Home" mask="11111111b">F10_524_ECE</function>
                <function start="160" end="175" comment="Remote Light" mask="11111111b">F10_524_ECE</function>
            </group>
            <group id="3006">
                <function start="16" end="31" comment="Seitenmarkierungsleuchte" mask="11111111b">F10_524_ECE</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001082" name="TMS_03" author="SaNGRia" series="F030,F080">
        <code description="Turn sidemarker LEDs OFF - Driver side. Step 1 of 2. See TMS-1083 (F3x and F8x)">
            <group id="3005">
                <function start="16" end="31" comment="Turn sidemarker LEDs OFF" mask="11111111b">00, 03, 00, 00, 00, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="32" end="47" comment="Turn sidemarker LEDs OFF" mask="11111111b">00, 03, 00, 00, 00, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="80" end="95" comment="Turn sidemarker LEDs OFF" mask="11111111b">00, 03, 00, 00, 00, 03, 00, 00, 64, 03, 00, 00, 2E, 04, 00, 00</function>
            </group>
        </code>
        <code description="Turn sidemarker LEDs ON - Driver side. Step 1 of 2. See TMS-1083 (F3x and F8x)">
            <group id="3005">
                <function start="16" end="31" comment="Turn sidemarker LEDs ON" mask="11111111b">00, 03, 00, 00, 64, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="32" end="47" comment="Turn sidemarker LEDs ON" mask="11111111b">00, 03, 00, 00, 64, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="80" end="95" comment="Turn sidemarker LEDs ON" mask="11111111b">00, 03, 00, 00, 64, 03, 00, 00, 64, 03, 00, 00, 2E, 04, 00, 00</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001083" name="TMS_03" author="SaNGRia" series="F010">
        <code description="Turn OFF Amber sidemarker lights. Part 2 of 2. See TMS41. (F10 LCI Bi-Xenon)">
            <group id="3005">
                <function start="16" end="31" comment="Standlicht Modus 1" mask="11111111b">F10_524_ECE</function>
                <function start="32" end="47" comment="Standlicht Modus 2" mask="11111111b">F10_524_ECE</function>
                <function start="48" end="63" comment="Standlicht Modus 3" mask="11111111b">F10_524_ECE</function>
                <function start="80" end="95" comment="Welcome Light 1" mask="11111111b">F10_524_ECE</function>
                <function start="144" end="159" comment="Follow Me Home" mask="11111111b">F10_524_ECE</function>
                <function start="160" end="175" comment="Remote Light" mask="11111111b">F10_524_ECE</function>
            </group>
            <group id="3006">
                <function start="16" end="31" comment="Seitenmarkierungsleuchte" mask="11111111b">F10_524_ECE</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001083" name="TMS_03" author="SaNGRia" series="F030,F080">
        <code description="Turn sidemarker LEDs OFF - Passenger side. Step 2 of 2. See TMS-1082 (F3x and F8x)">
            <group id="3005">
                <function start="16" end="31" comment="Turn sidemarker LEDs OFF" mask="11111111b">00, 03, 00, 00, 00, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="32" end="47" comment="Turn sidemarker LEDs OFF" mask="11111111b">00, 03, 00, 00, 00, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="80" end="95" comment="Turn sidemarker LEDs OFF" mask="11111111b">00, 03, 00, 00, 00, 03, 00, 00, 64, 03, 00, 00, 2E, 04, 00, 00</function>
            </group>
        </code>
        <code description="Turn sidemarker LEDs ON - Passenger side. Step 2 of 2. See TMS-1082 (F3x and F8x)">
            <group id="3005">
                <function start="16" end="31" comment="Turn sidemarker LEDs ON" mask="11111111b">00, 03, 00, 00, 64, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="32" end="47" comment="Turn sidemarker LEDs ON" mask="11111111b">00, 03, 00, 00, 64, 03, 00, 00, 64, 03, 00, 00, 2B, 04, 00, 00</function>
                <function start="80" end="95" comment="Turn sidemarker LEDs ON" mask="11111111b">00, 03, 00, 00, 64, 03, 00, 00, 64, 03, 00, 00, 2E, 04, 00, 00</function>
            </group>
        </code>
    </cafd>
    <cafd id="00000794" name="FEM_BODY" author="SaNGRia" series="F030,F080">
        <code description="F3x and F8x NGHB. Step 3 of 3. See LHM43/44.">
            <group id="3073">
                <function start="176" end="184" comment="NGHB PDF Step 3" mask="11111111b">00, 00, 00, 15, 00, 00, 0A, 15, 1F</function>
            </group>
            <group id="3074">
                <function start="81" end="86" comment="NGHB PDF Step 3" mask="11111111b">2E, 3B, 00, 00, 00, 00</function>
                <function start="87" end="92" comment="NGHB PDF Step 3" mask="11111111b">2E, 3B, 00, 00, 00, 00</function>
                <function start="93" end="98" comment="NGHB PDF Step 3" mask="11111111b">00, 00, 00, 00, 00, 00</function>
                <function start="99" end="104" comment="NGHB PDF Step 3" mask="11111111b">00, 00, 00, 00, 00, 00</function>
                <function start="60" end="60" comment="P3.59 improvement" mask="11111111b">27</function>
                <function start="61" end="61" comment="P3.59 improvement" mask="11111111b">1F</function>
                <function start="63" end="63" comment="P3.59 improvement" mask="11111111b">E1</function>
            </group>
        </code>
        <code description="ENABLE Unlock doors when STOP engine – if auto-locked">
            <group id="3040">
                <function start="1" end="1" comment="CLM_UNLOCK_KL15OFF_AFTER_PIA_AUTO_LOCK" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE FRONT Window Safety (Continued movement when doors opened). REM for Rear">
            <group id="3050">
                <function start="0" end="0" comment="FH_TUERAUF_STOP_MAUT" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Rear Tail-light with DRL (8TL). Part 1 of 2. See REM">
            <group id="3060">
                <function start="31" end="31" mask="00110000b">TFL_S</function>
            </group>
        </code>
        <code description="Reduce Automatic Headlamp Sensitivity">
            <group id="3130">
                <function start="5" end="5" mask="00000111b">unempfindlich</function>
            </group>
        </code>
        <code description="Increase Soft Triple Blinker to Five (5) (EXCLUDES P3.61.x)">
            <group id="3060">
                <function start="7" end="7" mask="00000111b">04</function>
            </group>
        </code>
        <code description="ENABLE EU Brake Light Behavior (Blink)">
            <group id="3060">
                <function start="16" end="16" mask="00000011b">bremslicht_blinkend</function>
            </group>
        </code>
        <code description="ENABLE Door Handle LED Lights while in reverse">
            <group id="3070">
                <function start="11" end="11" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Fog Lights with High Beams">
            <group id="3060">
                <function start="20" end="20" mask="00100000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Fog Lights with Parking Lights">
            <group id="3060">
                <function start="29" end="29" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="Separates Ambient Light Level and Instrument Cluster Light Level">
            <group id="3070">
                <function start="4" end="4" mask="10000000b" comment="AMBIENTE_NACHFUEHRUNG (default : aktiv)">nicht_aktiv</function>
            </group>
        </code>
        <code description="Open Windows/Fold Mirrors with Keyfob or CA (Newer I-Step)">
            <group id="3110">
                <function start="8" end="8" comment="ASP_AUSKLAPPEN_NACH_KOMFORTSCHLIESSEN" mask="00000001b">aktiv</function>
                <function start="1" end="1" comment="ASP_BEIKLAPPEN_BEI_KOMFORTSCHLIESSEN" mask="00000001b">aktiv</function>
            </group>
            <group id="3053">
                <function start="0" end="0" comment="KOMFORTSCHLIESSUNG_FB" mask="10000000b">aktiv</function>
                <function start="0" end="0" comment="KOMFORTOEFFNUNG_FB" mask="01000000b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTOEFFNUNG" mask="00000001b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTSCHLIESSUNG" mask="00000010b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTSCHLIESSUNG_PA" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="Open Windows/Fold Mirrors with Keyfob or CA (Older I-Step)">
            <group id="3110">
                <function start="7" end="7" comment="ASP_AUSKLAPPEN_NACH_KOMFORTSCHLIESSEN" mask="00000001b">aktiv</function>
                <function start="0" end="0" comment="ASP_BEIKLAPPEN_BEI_KOMFORTSCHLIESSEN" mask="10000000b">aktiv</function>
            </group>
            <group id="3053">
                <function start="0" end="0" comment="KOMFORTSCHLIESSUNG_FB" mask="10000000b">aktiv</function>
                <function start="0" end="0" comment="KOMFORTOEFFNUNG_FB" mask="01000000b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTOEFFNUNG" mask="00000001b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTSCHLIESSUNG" mask="00000010b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTSCHLIESSUNG_PA" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="Remove open/close window and mirror initiation delay">
            <group id="3053">
                <function start="9" end="9" comment="KOMFORT_SCHLIESSEN" mask="11111111b">00</function>
            </group>
        </code>
        <code description="Removes Trunk Opening Delay - 0 seconds (Older I-Step)">
            <group id="3040">
                <function start="10" end="10" comment="CLM_TIMEOUT_HK_SMO" mask="11111111b">00</function>
            </group>
        </code>
        <code description="Removes Trunk Opening Delay - 0 seconds (Newer I-Step)">
            <group id="3040">
                <function start="6" end="6" comment="CLM_TIME_DELAY_BOOTLID" mask="11111111b">00</function>
            </group>
        </code>
        <code description="Turn off taillight flashing when opening trunk via Comfort Access">
            <group id="3040">
                <function start="2" end="2" comment="CLM_SMO_INDICATOR" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="Turn On LED Fog Lights with Welcome Lights">
            <group id="3063">
                <function start="55" end="55" comment="MAPPING_NEBELSCHW_L_PART_OF_WL" mask="11000000b">01</function>
                <function start="66" end="66" comment="MAPPING_NEBELSCHW_R_PART_OF_WL" mask="11000000b">01</function>
            </group>
        </code>
        <code description="ENABLE Increased Passenger Mirror Tilt (Curb View) in Reverse (OLD FIRMWARE)">
            <group id="3110">
                <function start="1" end="1" comment="ASP_BORDSTEINAUTOMATIK_DELTA" mask="11111111b">5A</function>
            </group>
        </code>
        <code description="ENABLE Increased Passenger Mirror Tilt (Curb View) in Reverse (P3.61.2)">
            <group id="3110">
                <function start="2" end="2" comment="ASP_BORDSTEINAUTOMATIK_DELTA" mask="11111111b">5A</function>
            </group>
        </code>
        <code description="ENABLE Smart Trunk Closing (Requires 322, 316, and 11-14 Prod Date">
            <group id="3030">
                <function start="5" end="5" comment="CAM_SMART_CLOSER" mask="00000110b">01</function>
            </group>
        </code>
    </cafd>
    <cafd id="000007A1" name="REM_01" author="SaNGRia" series="F030">
        <code description="ENABLE Rear Tail-light with DRL. Part 2 of 2. See FEM_BODY">
            <group id="3062">
                <function start="220" end="220" comment="Turns On Left Tail-light (Inner Part) on with DRL" mask="00111111b">sl_2_l</function>
                <function start="230" end="230" comment="Turns On Right Tail-light (Inner Part) on with DRL" mask="00111111b">sl_2_r</function>
                <function start="200" end="200" comment="Turns On Left Tail-light (Outer Part) on with DRL" mask="00111111b">sl_l</function>
                <function start="210" end="210" comment="Turns On Right Tail-light (Outer Part) on with DRL" mask="00111111b">sl_r</function>
            </group>
        </code>
        <code description="ENABLE REAR windows roll up while doors opened. FEM for Front">
            <group id="3050">
                <function start="0" end="0" comment="FH_TUERAUF_STOP_MAUT" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Top/Rear camera at any speed. See TRSVC for Side View">
            <group id="3203">
                <function start="7" end="7" comment="The speed when it auto disables top camera view" mask="11111111b">FF</function>
                <function start="8" end="8" comment="The speed when it auto disables rear camera view" mask="11111111b">FF</function>
                <function start="9" end="9" comment="The distance when it auto disables top camera view" mask="11111111b">FF</function>
                <function start="10" end="10" comment="The distance when it auto disables rear camera view" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Outer Light Flashing with EU Brake Force - LED Only">
            <group id="3062">
                <function start="110" end="110" comment="MAPPING_BRAKEFORCED_L_OUTPUT" mask="00111111b">bl_l</function>
                <function start="120" end="120" comment="MAPPING_BRAKEFORCED_R_OUTPUT" mask="00111111b">bl_r</function>
            </group>
        </code>
        <code description="Increase Outer Light Flashing with EU Brake Force - LED Only">
            <group id="3064">
                <function start="17" end="17" comment="ESS_BLINKFREQ_1" mask="00001110b">05</function>
                <function start="17" end="17" comment="ESS_BLINKFREQ_2" mask="01110000b">05</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001A33" name="DSC" author="SaNGRia" series="F080">
        <code description="Euro MDM (P3.59.2 Settings): Coding US Spec Cars (F80/F82)">
            <group id="3000">
                <function start="12" end="12" comment="C_Laenderkennung. ONLY Needed Change" mask="00000011b">ECE</function>
            </group>
            <group id="3004">
                <function start="14" end="14" comment="C_AMR_2_c" mask="11110000b">00</function>
                <function start="15" end="15" comment="C_AMR_3_c" mask="00001111b">00</function>
            </group>
            <group id="3008">
                <function start="3" end="3" comment="CTpmsMarket" mask="00000010b">01</function>
                <function start="3" end="3" comment="CPrewarnENABLE" mask="00000010b">00</function>
                <function start="3" end="3" comment="CPrewarnIgnition" mask="00010000b">00</function>
                <function start="4" end="4" comment="MinRcpf" mask="11111111b">50</function>
                <function start="5" end="5" comment="MinRcpr" mask="11111111b">50</function>
                <function start="6" end="6" comment="CalLrPDevMax" mask="11111111b">28</function>
                <function start="7" end="7" comment="CPInitRangeMax" mask="11111111b">50</function>
                <function start="8" end="8" comment="UiaSetLevelPc" mask="11111111b">19</function>
                <function start="11" end="11" comment="UiwSetLevelPc" mask="11111111b">14</function>
                <function start="13" end="13" comment="UiwSetLevelDistMin" mask="11111111b">0C</function>
                <function start="16" end="16" comment="CalTimeConfUiw" mask="11111111b">0A</function>
                <function start="17" end="17" comment="CDtAmbPrewarn" mask="11111111b">0A</function>
                <function start="19" end="19" comment="CTRefShift" mask="11111111b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="000017BC" name="BDC_01" author="SaNGRia" series="G011,G030">
        <code description="ENABLE Mirrors Fold/Windows Roll Up with CA and KeyFOB. Part 1 of 2. See IDF7">
            <group id="3110">
                <function start="0" end="0" comment="ASP_AUSKLAPPEN_NACH_KOMFORTSCHLIESSEN" mask="00000010b">aktiv</function>
                <function start="0" end="0" comment="ASP_BEIKLAPPEN_BEI_KOMFORTSCHLIESSEN" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="Unlock doors when STOP engine - auto or manual lock">
            <group id="3041">
                <function start="42" end="42" comment="CLI_DEFAULT_UNLOCK_AFTER_END_OF_DRIVING" mask="00001100b">aktiv</function>
            </group>
        </code>
        <code description="Unlock doors when STOP engine - auto lock">
            <group id="3041">
                <function start="42" end="42" comment="CLI_DEFAULT_UNLOCK_AFTER_END_OF_DRIVING" mask="00001100b">nur_nach_v_verriegeln</function>
            </group>
        </code>
        <code description="ENABLE Fog Lights with High Beams">
            <group id="3075">
                <function start="12" end="12" comment="NSW_AUS_BEI_FL" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Fog Lights with Parking Lights and High Beams">
            <group id="3075">
                <function start="12" end="12" comment="NSW_AUS_BEI_FL" mask="00000001b">nicht_aktiv</function>
                <function start="12" end="12" comment="NSW_EIN_AUF_LDS_STL" mask="00000010b">aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001DF7" name="BDC_01" author="SaNGRia" series="G011,G030">
        <code description="ENABLE Front Window Roll Up when doors opened">
            <group id="3510">
                <function start="0" end="0" comment="FH_TUERAUF_STOP_MAUT" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="Allow Rear Window Roll Up when doors opened">
            <group id="3511">
                <function start="0" end="0" comment="FH_TUERAUF_STOP_MAUT_REAR" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Mirrors Fold/Windows Roll Up with CA and KeyFOB. Part 2 of 2. See 17BC">
            <group id="3514">
                <function start="0" end="0" comment="KOMFORTOEFFNUG_FB" mask="01000000b">aktiv</function>
                <function start="0" end="0" comment="KOMFORTSCHLIESSUNG_FB" mask="10000000b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTOEFFNUG" mask="00000001b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTSCHLIESSUNG" mask="00000010b">aktiv</function>
                <function start="1" end="1" comment="KOMFORTSCHLIESSUNG_PA" mask="00000100b">aktiv</function>
            </group>
        </code>
        <code description="Remove Mirror/Window Initiation Delay with CA and KeyFOB">
            <group id="3514">
                <function start="10" end="10" comment="KOMFORT_SCHLIESSEN" mask="11111111b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="00002098" name="HKFM_2015" author="SaNGRia" series="F015,G001,G011,G030,RR11">
        <code description="ENABLE  Trunk or Tailgate CLOSE with KeyFOB or RockerSwitch (No HOLD)">
            <group id="300B">
                <function start="1" end="1" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_BUTTON_TYPE" mask="11111111b">05</function>
            </group>
            <group id="3008">
                <function start="1" end="1" comment="HKL_ROCKERSWITCHPOS1_BUTTON_TYPE" mask="11111111b">05</function>
            </group>
        </code>
        <code description="ENABLE Long Press (HOLD) While Close Trunk with RockerSwitch">
            <group id="3008">
                <function start="0" end="0" comment="HKL_ROCKERSWITCHPOS1_LONGPRESS_CLOSE" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE Long Press (HOLD) While Close Trunk with RockerSwitch">
            <group id="3008">
                <function start="0" end="0" comment="HKL_ROCKERSWITCHPOS1_LONGPRESS_CLOSE" mask="00001000b">00</function>
            </group>
        </code>
        <code description="ENABLE Long Press (HOLD) Close Trunk with KeyFOB">
            <group id="300B">
                <function start="0" end="0" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_LONGPRESS_CLOSE" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE Long Press (HOLD) Close Trunk with KeyFOB">
            <group id="300B">
                <function start="0" end="0" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_LONGPRESS_CLOSE" mask="00001000b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="0000570E" name="HKFM_2015" author="SaNGRia" series="F015,G001,G011,G030,RR11">
        <code description="ENABLE  Trunk or Tailgate CLOSE with KeyFOB or RockerSwitch (No HOLD)">
            <group id="300B">
                <function start="1" end="1" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_BUTTON_TYPE" mask="11111111b">05</function>
            </group>
            <group id="3008">
                <function start="1" end="1" comment="HKL_ROCKERSWITCHPOS1_BUTTON_TYPE" mask="11111111b">05</function>
            </group>
        </code>
        <code description="ENABLE Long Press (HOLD) While Close Trunk with RockerSwitch">
            <group id="3008">
                <function start="0" end="0" comment="HKL_ROCKERSWITCHPOS1_LONGPRESS_CLOSE" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE Long Press (HOLD) While Close Trunk with RockerSwitch">
            <group id="3008">
                <function start="0" end="0" comment="HKL_ROCKERSWITCHPOS1_LONGPRESS_CLOSE" mask="00001000b">00</function>
            </group>
        </code>
        <code description="ENABLE Long Press (HOLD) Close Trunk with KeyFOB">
            <group id="300B">
                <function start="0" end="0" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_LONGPRESS_CLOSE" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE Long Press (HOLD) Close Trunk with KeyFOB">
            <group id="300B">
                <function start="0" end="0" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_LONGPRESS_CLOSE" mask="00001000b">00</function>
            </group>
        </code>
    </cafd>
    <cafd id="00005710" name="HKFM_2015" author="SaNGRia" series="F015,G001,G011,G030,RR11">
        <code description="ENABLE  Trunk or Tailgate CLOSE with KeyFOB or RockerSwitch (No HOLD)">
            <group id="300B">
                <function start="1" end="1" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_BUTTON_TYPE" mask="11111111b">05</function>
            </group>
            <group id="3008">
                <function start="1" end="1" comment="HKL_ROCKERSWITCHPOS1_BUTTON_TYPE" mask="11111111b">05</function>
            </group>
        </code>
        <code description="ENABLE Long Press (HOLD) While Close Trunk with RockerSwitch">
            <group id="3008">
                <function start="0" end="0" comment="HKL_ROCKERSWITCHPOS1_LONGPRESS_CLOSE" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE Long Press (HOLD) While Close Trunk with RockerSwitch">
            <group id="3008">
                <function start="0" end="0" comment="HKL_ROCKERSWITCHPOS1_LONGPRESS_CLOSE" mask="00001000b">00</function>
            </group>
        </code>
        <code description="ENABLE Long Press (HOLD) Close Trunk with KeyFOB">
            <group id="300B">
                <function start="0" end="0" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_LONGPRESS_CLOSE" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE Long Press (HOLD) Close Trunk with KeyFOB">
            <group id="300B">
                <function start="0" end="0" comment="HKL_REMOTECONTROLLIFTGATEBUTTON_LONGPRESS_CLOSE" mask="00001000b">00</function>
            </group>
        </code>
    </cafd>    
    <cafd id="000022D3" name="IHKA_PR01" author="SaNGRia" series="G011,G030">
        <code description="ENABLE HVAC memory - A/C stay OFF if OFF at vehicle shutdown">
            <group id="3003">
                <function start="0" end="0" comment="OFF_MEMORY" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Air Re-Circulation memory - Remembers shutdown Setting">
            <group id="3003">
                <function start="0" end="0" comment="MEMORY_UMLUFT" mask="00000010b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE A/C from turning ON if Auto Button is pressed ">
            <group id="3003">
                <function start="0" end="0" comment="AC_ON_WITH_AUTO" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001B29" name="ACSM_5" author="SaNGRia" series="G011,G030">
        <code description="DISABLE Seat Belt Status in Cluster (Passenger) - 2016 Firmware">
            <group id="3001">
                <function start="6" end="6" comment="Gurtzustandsanzeige_Beifahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Status in Cluster (Driver) - 2016 Firmware">
            <group id="3001">
                <function start="5" end="5" comment="Gurtzustandsanzeige_Fahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder Chime (Driver) - 2016 Firmware">
            <group id="3001">
                <function start="1" end="1" comment="SeatBeltReminder_Fahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Reminder (Passenger) - 2016 Firmware">
            <group id="3001">
                <function start="2" end="2" comment="SeatBeltReminder_Beifahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Disconnected Reminder Sound (Driver) - 2016 Firmware">
            <group id="3001">
                <function start="3" end="3" comment="SBR_PreWarning_Fahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Seat Belt Disconnected Reminder Sound (Passenger) - 2016 Firmware">
            <group id="3001">
                <function start="4" end="4" comment="SBR_PreWarning_Beifahrer" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Initial Belt Warning Gong - 2016 Firmware">
            <group id="3001">
                <function start="0" end="0" comment="Initialwarnung" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
    </cafd>
    <cafd id="00001EF6" name="HU_NBT_EVO" author="SaNGRia" series="F015,F030,G011">
        <code description="ENABLE Video in Motion (VIM) - Only ID4 (Any Speed)">
            <group id="3000">
                <function start="5" end="5" comment="VIDEO_HANDBRAKE" mask="00000100b">nicht_aktiv</function>
                <function start="5" end="5" comment="VIDEO_FRONT_LOCKED" mask="00010000b">nicht_aktiv</function>
                <function start="2" end="2" comment="VIDEO_SPEEDLOCK_CONDITION" mask="00000111b">none</function>
                <function start="146" end="146" comment="SPEEDLOCK_SPEEDVALUE_MIN" mask="00011111b">nicht_aktiv</function>
                <function start="147" end="147" comment="SPEEDLOCK_SPEEDVALUE_MAX" mask="00111111b">nicht_aktiv</function>
            </group>
            <group id="3006">
                <function start="25" end="25" comment="SPEEDLOCK_X_KMH_MIN" mask="11111111b">FF</function>
                <function start="26" end="26" comment="SPEEDLOCK_X_KMH_MAX" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Video in Motion (VIM) - only 1D5 (Up to 63 kph)">
            <group id="3000">
                <function start="5" end="5" comment="VIDEO_HANDBRAKE" mask="00000100b">nicht_aktiv</function>
                <function start="5" end="5" comment="VIDEO_FRONT_LOCKED" mask="00010000b">nicht_aktiv</function>
                <function start="2" end="2" comment="VIDEO_SPEEDLOCK_CONDITION" mask="00000111b">none</function>
                <function start="146" end="146" comment="SPEEDLOCK_SPEEDVALUE_MIN" mask="00011111b">1F</function>
                <function start="147" end="147" comment="SPEEDLOCK_SPEEDVALUE_MAX" mask="00111111b">3F</function>
            </group>
            <group id="3006">
                <function start="25" end="25" comment="SPEEDLOCK_X_KMH_MIN" mask="11111111b">FF</function>
                <function start="26" end="26" comment="SPEEDLOCK_X_KMH_MAX" mask="11111111b">FF</function>
            </group>
        </code>
        <code description="ENABLE Call Log Timestamp">
            <group id="3003">
                <function start="1" end="1" comment="TIMESTAMP_DISPLAY" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="Displays entire text (SMS) message on iDrive">
            <group id="3003">
                <function start="11" end="11" comment="PIM_Driving_Text_Length" mask="00000111b">whole_text</function>
            </group>
            <group id="3000">
                <function start="31" end="31" comment="SPEEDLOCK_TEXT_LENGTH" mask="00111000b">whole_text</function>
                <function start="137" end="137" comment="MYINFO_DRIVING_TEXT_LENGTH" mask="00011100b">whole_text</function>
                <function start="137" end="137" comment="AKD_DRIVING_TEXT_LENGTH" mask="11100000b">whole_text</function>
                <function start="138" end="138" comment="BMWINFO_DRIVING_TEXT_LENGTH" mask="00000111b">whole_text</function>
            </group>
        </code>
        <code description="ENABLE HUD Turnsignal. Part 1 of 2. Go to KOMBI. (Excludes 6WB)">
            <group id="300C">
                <function start="0" end="0" comment="HUD_TURNSIGNAL" mask="01000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Lock/Unlock Sound Confirm Checkbox With alarm only">
            <group id="3000">
                <function start="110" end="110" comment="Acoustical_lock_confirm" mask="00000001b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Lock/Unlock Sound Confirm Checkbox With alarm only">
            <group id="3000">
                <function start="110" end="110" comment="Acoustical_lock_confirm" mask="00000001b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Sports Displays - Red/Silver.">
            <group id="3000">
                <function start="133" end="133" comment="M_VEHICLE" mask="01000000b">aktiv</function>
            </group>
            <group id="3009">
                <function start="9" end="9" comment="EFF_DYN_SPORT_UNIT" mask="00010000b">aktiv</function>
                <function start="9" end="9" comment="EFF_DYN_SPORT_CID" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Sports Displays - Amber Standard.">
            <group id="3000">
                <function start="133" end="133" comment="M_VEHICLE" mask="01000000b">nicht_aktiv</function>
            </group>
            <group id="3009">
                <function start="9" end="9" comment="EFF_DYN_SPORT_UNIT" mask="00010000b">aktiv</function>
                <function start="9" end="9" comment="EFF_DYN_SPORT_CID" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Office/Service Message Function Speed Lock-Out">
            <group id="3000">
                <function start="136" end="136" comment="OFFICE_MESSAGES_SPEEDLOCK_CONDITION" mask="00111000b">none</function>
                <function start="138" end="138" comment="SERVICES_MESSAGES_SPEEDLOCK_CONDITION" mask="00111000b">none</function>
            </group>
        </code>
        <code description="ENABLE IDrive DRL-selectable menu item (8TN US Typecode)">
            <group id="3000">
                <function start="92" end="92" comment="DAYDRIVING_LIGHT" mask="00011000b">standard</function>
            </group>
        </code>
        <code description="ENABLE British Voice on Navigation. Part 1 of 2. See KOMBI (ID4 ONLY)">
            <group id="3007">
                <function start="0" end="0" comment="LANGUAGE_ENGLISH_UK" mask="00001100b">master</function>
                <function start="0" end="0" comment="LANGUAGE_ENGLISH_US" mask="00110000b">nicht_aktiv</function>
            </group>
            <group id="3006">
                <function start="0" end="0" comment="NAVI_DESTINATION_INPUT_US" mask="00000100b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Default Time settings to 24H">
            <group id="3004">
                <function start="8" end="8" comment="DEFAULT_ZEIT_EINHEIT" mask="00010000b">24h</function>
            </group>
        </code>
        <code description="Allows volume to be retained up to 100% rather than startup at 25%">
            <group id="3002">
                <function start="3" end="3" comment="VOL_MAX_ON" mask="11111111b">32</function>
            </group>
        </code>
        <code description="ENABLE Owners Manual in Motion (ID4 ONLY)">
            <group id="3000">
                <function start="0" end="0" comment="SL06_IBA_1" mask="00100000b">nicht_aktiv</function>
                <function start="0" end="0" comment="SL07_IBA_2" mask="01000000b">nicht_aktiv</function>
                <function start="2" end="2" comment="SL21_IBA_3" mask="00010000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE All Video Codecs and Video Import">
            <group id="3000">
                <function start="15" end="15" comment="ENT_CODEC_OGG" mask="00010000b">aktiv</function>
                <function start="15" end="15" comment="ENT_CODEC_XVID" mask="00100000b">aktiv</function>
                <function start="15" end="15" comment="ENT_CODEC_VCD" mask="01000000b">aktiv</function>
                <function start="13" end="13" comment="ENT_MC_VIDEO_SUPPORT" mask="00000100b">Aktiv</function>
                <function start="32" end="32" comment="API_USB_VIDEO" mask="00000110b">both</function>
            </group>
        </code>
        <code description="M Performance Start Animation of HMI">
            <group id="3001">
                <function start="62" end="62" comment="STARTUP_TYPE" mask="00000110b">animation</function>
                <function start="62" end="62" comment="STARTUP_EMBLEM" mask="01111000b">variant_01</function>
            </group>
        </code>
        <code description="DISABLE STARTUP/CAMERA Legal Disclaimers">
            <group id="3001">
                <function start="58" end="58" comment="LEGAL_DISCLAIMER_TIME" mask="11111111b">00</function>
                <function start="52" end="52" comment="MACRO_CAM_LEGALDISCLAIMER" mask="11111111b">00</function>
                <function start="53" end="53" comment="MACRO_NIVICAM_LDISCLAIMER" mask="11111111b">00</function>
            </group>
        </code>
        <code description="Show Tire Pressure and Temperature in iDrive">
            <group id="3001">
                <function start="1" end="1" comment="RDC_SAFETY" mask="00100000b">aktiv</function>
                <function start="66" end="66" comment="RDC_DRUCK_TEMP" mask="00001100b">druck_und_temperatur</function>
            </group>
        </code>
        <code description="ENABLE Trip Import via USB">
            <group id="3006">
                <function start="3" end="3" comment="navi_trip_import" mask="00000001b">aktiv</function>
                <function start="3" end="3" comment="navi_dest_import" mask="00000100b">aktiv</function>
                <function start="3" end="3" comment="navi_mypoi_import" mask="00010000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Rear Camera Zoom -Trailer Mode-">
            <group id="3001">
                <function start="54" end="54" comment="macro_trailer_coupling" mask="00000001b">Aktiv</function>
            </group>
        </code>
        <code description="ENABLE Transfer of Phone Ringtone to Vehicle (Iphone Only)">
            <group id="3003">
                <function start="6" end="6" comment="INBAND_RINGING" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE AM Radio on Hybrid Vehicles (F15/I12/I01)">
            <group id="3002">
                <function start="52" end="52" comment="RADIO_BAND_KW" mask="00001000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Bluetooth Device and NFC Pairing and Beam Speedlock">
            <group id="3000">
                <function start="12" end="12" comment="NFC_BT_PAIRING_SPEEDLOCK" mask="00001000b">nicht_aktiv</function>
                <function start="12" end="12" comment="NFC_BEAM_SPEEDLOCK" mask="00010000b">nicht_aktiv</function>
                <function start="1" end="1" comment="SL16_ADD_CEDEVICE" mask="10000000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="DISABLE Bluetooth Device and NFC Pairing and Beam Speedlock (Untested)">
            <group id="3000">
                <function start="12" end="12" comment="NFC_BT_PAIRING_SPEEDLOCK" mask="00001000b">aktiv</function>
                <function start="12" end="12" comment="NFC_BEAM_SPEEDLOCK" mask="00010000b">aktiv</function>
                <function start="1" end="1" comment="SL16_ADD_CEDEVICE" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE Speller Touchpad Speedlock">
            <group id="3000">
                <function start="31" end="31" comment="SPEEDLOCK_SPELLER_INPUT" mask="00000111b">none_locked</function>
            </group>
        </code>
        <code description="ENABLE MIRACAST Function. See WLAN">
            <group id="3000">
                <function start="6" end="6" comment="ENT_MIRACAST" mask="10000000b">aktiv</function>
                <function start="13" end="13" comment="ENT_MC_WLAN_STREAM_DMP" mask="10000000b">aktiv</function>
                <function start="30" end="30" comment="ENT_MIRACAST_DISPLAY_SETTINGS" mask="00001000b">aktiv</function>
            </group>
            <group id="3003">
                <function start="21" end="21" comment="WLAN_WIFI_DIRECT" mask="00000010b">aktiv</function>
                <function start="20" end="20" comment="WLAN_STATUS" mask="10000000b">aktiv</function>
            </group>
        </code>
        <code description="DISABLE MIRACAST Display Settings">
            <group id="3000">
                <function start="30" end="30" comment="ENT_MIRACAST_DISPLAY_SETTINGS" mask="00001000b">nicht_aktiv</function>
            </group>
        </code>
        <code description="ENABLE Album Cover Scale to Full-Size">
            <group id="3000">
                <function start="14" end="14" comment="ENT_MC_COVER_SCALE" mask="00100000b">aktiv</function>
            </group>
        </code>
        <code description="ENABLE Hold-Mode for Range Extender (I001/1012)">
            <group id="3009">
                <function start="4" end="4" comment="EV_MENU_AVAILABLE" mask="01100000b">rex</function>
            </group>
        </code>
        <code description="DISABLE Radio Tuner Speedlock">
            <group id="3000">
                <function start="109" end="109" comment="SPEEDLOCK_HMI_TUNER" mask="00000001b">00</function>
            </group>
        </code>
        <code description="Changes Fueling POI to ONLY CHARGING Station (Default = Petrol + Diesel)">
            <group id="3006">
                <function start="30" end="30" comment="CAR_TYPE_POI = Charge" mask="00000011b">00</function>
            </group>
        </code>
        <code description="Changes Fueling POI to ONLY GAS and Diesel (iDefault = Also Charge Station)">
            <group id="3006">
                <function start="30" end="30" comment="CAR_TYPE_POI = Petrol + Gas" mask="00000011b">01</function>
            </group>
        </code>
        <code description="ENABLE Automatic Time Setting by NAV GPS (Fixes Time Zone Adjustment)">
            <group id="3000">
                <function start="19" end="19" comment="Default = BMW Online" mask="00000110b">02</function>
            </group>
        </code>
        <code description="ENABLE IDrive Configurable Mirror Folding (G12 and G30 Only. Req 11-16 Firmware)">
            <group id="3000">
                <function start="36" end="36" comment="SETTINGS_AUTOMATIC_EXT_MIRROR_FOLDING" mask="10000000b">01</function>
            </group>
        </code>
        <code description="ENABLE 6NW Wireless Charge Forgot Phone Warning Reminder (IDrive Configured. Testing)">
            <group id="3000">
                <function start="23" end="23" comment="WCA" mask="00001000b">01</function>
            </group>
        </code>
        <code description="DISABLE 6NW Wireless Charge Forgot Phone Warning Reminder (IDrive Configured)">
            <group id="3000">
                <function start="23" end="23" comment="WCA" mask="00001000b">00</function>
            </group>
        </code>
        <code description="Change Played Sound Signal Set (BMW)">
            <group id="3002">
                <function start="26" end="26" comment="SOUND_SIGNAL_SET" mask="00111000b">00</function>
            </group>
        </code>
        <code description="Change Played Sound Signal Set (mini)">
            <group id="3002">
                <function start="26" end="26" comment="SOUND_SIGNAL_SET" mask="00111000b">01</function>
            </group>
        </code>
        <code description="Change Played Sound Signal Set (Rolls Royce)">
            <group id="3002">
                <function start="26" end="26" comment="SOUND_SIGNAL_SET" mask="00111000b">02</function>
            </group>
        </code>
        <code description="Change Played Sound Signal Set (BMW_i)">
            <group id="3002">
                <function start="26" end="26" comment="SOUND_SIGNAL_SET" mask="00111000b">03</function>
            </group>
        </code>
    </cafd>
    <cafd id="00002089" name="KAFAS3" author="SaNGRia" series="G011">
        <code description="ENABLE EU SLI sign (White circle with Red outline)">
            <group id="3010">
                <function start="4" end="4" comment="COUNTRY_CODING_DISPLAY" mask="11111111b">00</function>
            </group>
        </code>
    </cafd>
  
    <!--2022-02-03 Added aSLA, TLA, and DAP-->
	<!--Special Thanks to eaglesrest and atomantmk -->
    
    <cafd id="00003E52" name="HU_MGU" author="SaNGRia" series="G005, G007, G020, G015, G030, G011">	
		<code description="ENABLE Auto Speed Limit Assist (aSLA). Req ID7 and 11-20 I-Step. See 7083, SAS3 42C1, DSC 3D14 (2/4)">
			<group id="300A">
				<function start="10" end="10" comment="STRECKENVERLAUF - gen_01" mask="10000000b">01</function>
				<function start="13" end="13" comment="VORAUSSCHAU - gen_01" mask="00001100b">01</function>
				<function start="14" end="14" comment="SLAAUTOMATISCH - gen_01" mask="00110000b">01</function>
				<function start="14" end="14" comment="VOFFSET - gen_1" mask="11000000b">01</function>
				<function start="15" end="15" comment="VOFFSET_LANGSAM - gen_1" mask="11000000b">01</function>
				<function start="18" end="18" comment="STRECKENVERLAUF_GENERATION - gen_1" mask="00000011b">01</function>
			</group>	
		</code>	
		<code description="DISABLE Auto Speed Limit Assist (aSLA). See 7083, SAS3 42C1, DSC 3D14 (2/4)">
			<group id="300A">
				<function start="10" end="10" comment="STRECKENVERLAUF - gen_01" mask="10000000b">01</function>
				<function start="13" end="13" comment="VORAUSSCHAU - gen_01" mask="00001100b">00</function>
				<function start="14" end="14" comment="SLAAUTOMATISCH - gen_01" mask="00110000b">00</function>
				<function start="14" end="14" comment="VOFFSET - gen_1" mask="11000000b">00</function>
				<function start="15" end="15" comment="VOFFSET_LANGSAM - gen_1" mask="11000000b">00</function>
				<function start="18" end="18" comment="STRECKENVERLAUF_GENERATION - gen_1" mask="00000011b">01</function>
			</group>	
		</code>	
		<code description="ENABLE Traffic Light Assistant (TLA). Req ID7, 11-20 I-Step, and aSLA. See 7083, SAS3 42C1, DSC 3D14 (2/4)">
			<group id="300A">
				<function start="16" end="16" comment="AMPELN - gen_01" mask="01100000b">01</function>
				<function start="17" end="17" comment="AMPELASSISTENT - gen_01" mask="00110000b">01</function>
				<function start="17" end="17" comment="ANFAHRERINNERUNG - gen_01" mask="11000000b">01</function>
			</group>	
		</code>	
		<code description="DISABLE Traffic Light Assistant (TLA). See 7083, SAS3 42C1, DSC 3D14 (2/4)">
			<group id="300A">
				<function start="16" end="16" comment="AMPELN - gen_01" mask="01100000b">00</function>
				<function start="17" end="17" comment="AMPELASSISTENT - gen_01" mask="00110000b">00</function>
				<function start="17" end="17" comment="ANFAHRERINNERUNG - gen_01" mask="11000000b">00</function>
			</group>	
		</code>	
		<code description="ENABLE Driver Assistant Pro (DAP) - New Features. See BDC, SAS3 (2/3)">
			<group id="300A">
				<function start="14" end="14" comment="EINSEITIGVORBEIFAHREN - Undertaking gen_1" mask="00000011b">01</function>
				<function start="19" end="19" comment="RETTUNGSGASSE - Emergency Lane Formation aktiv" mask="00000100b">01</function>
				<function start="16" end="16" comment="SITUATIVERABSTAND - Adjust Distance Menu gen_1" mask="00000110b">01</function>
			</group>	
		</code>	
		<code description="DISABLE Driver Assistant Pro (DAP) - New Features. See BDC, SAS3 (2/3)">
			<group id="300A">
				<function start="14" end="14" comment="EINSEITIGVORBEIFAHREN - Undertaking gen_1" mask="00000011b">00</function>
				<function start="19" end="19" comment="RETTUNGSGASSE - Emergency Lane Formation aktiv" mask="00000100b">00</function>
				<function start="16" end="16" comment="SITUATIVERABSTAND - Adjust Distance Menu gen_1" mask="00000110b">01</function>
			</group>	
		</code>	
	</cafd>	
    <cafd id="000042C1" name="SAS3" author="SaNGRia" series="G005, G007, G020, G015, G030, G011">	
		<code description="ENABLE Auto Speed Limit Assist (aSLA). Req ID7 and 11-20 I-Step. See 7083, MGU, DSC 3D14 (3/4)">
			<group id="3001">
				<function start="167" end="167" comment="C_SLA_Anzeige_Zusatztexte - Nr001_aktiviert" mask="11111111b">01</function>
			</group>
			<group id="3000">	
				<function start="93" end="93" comment="C_SLA_Streckenregelung_vorhanden - NR_002_vorhanden_SLA_entkoppelt" mask="11111111b">02</function>
				<function start="112" end="115" comment="C_SLA_aSLA_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="116" end="119" comment="C_SLA_Vorausschau_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="130" end="130" comment="C_SLA_aSLA_vorhanden - Nr001_vorhanden" mask="11111111b">01</function>
				<function start="131" end="134" comment="C_SLA_Streckenregelung_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Auto Speed Limit Assist (aSLA). See 7083, MGU, DSC 3D14 (3/4)">
			<group id="3001">
				<function start="167" end="167" comment="C_SLA_Anzeige_Zusatztexte - Nr001_aktiviert" mask="11111111b">01</function>
			</group>
			<group id="3000">	
				<function start="93" end="93" comment="C_SLA_Streckenregelung_vorhanden - NR_002_vorhanden_SLA_entkoppelt" mask="11111111b">02</function>
				<function start="112" end="115" comment="C_SLA_aSLA_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">F9, 0F, 86, 00</function>
				<function start="116" end="119" comment="C_SLA_Vorausschau_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FB, DF, A7, C0</function>
				<function start="130" end="130" comment="C_SLA_aSLA_vorhanden - Nr001_vorhanden" mask="11111111b">00</function>
				<function start="131" end="134" comment="C_SLA_Streckenregelung_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, CF, 9F, F8</function>
			</group>	
		</code>	
		<code description="ENABLE Traffic Light Assistant (TLA). Req ID7, 11-20 I-Step, and aSLA. See 7083, MGU, DSC 3D14 (3/4)">
			<group id="3000">
				<function start="178" end="178" comment="C_UCC_vorhanden - Nr001_vorhanden" mask="11111111b">01</function>
				<function start="179" end="182" comment="C_SLA_UCC_Land_aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="188" end="191" comment="C_SLA_aUCC_Land_aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Traffic Light Assistant (TLA). See 7083, MGU, DSC 3D14 (3/4)">
			<group id="3000">
				<function start="178" end="178" comment="C_UCC_vorhanden - Nr000_nicht_vorhanden" mask="11111111b">00</function>
				<function start="179" end="182" comment="C_SLA_UCC_Land_aktiv - 0xFFFFFFFF" mask="11111111b">08, 00, 00, 00</function>
				<function start="188" end="191" comment="C_SLA_aUCC_Land_aktiv - 0xFFFFFFFF" mask="11111111b">08, 00, 00, 00</function>
			</group>	
		</code>	
		<code description="ENABLE Driver Assistant Pro (DAP) - Unsupported Highway Exit Assistant. See BDC, MGU (3/3)">
			<group id="3000">
				<function start="183" end="183" comment="C_QmaN_Vorhanden - nr001_vorhanden" mask="11111111b">00</function>
				<function start="184" end="187" comment="C_SLA_QmaN_Land_aktiv - FFFFFFFF" mask="11111111b">FA, C3, 81, F8</function>
			</group>	
		</code>	
		<code description="DISABLE Driver Assistant Pro (DAP) - Unsupported Highway Exit Assistant. See BDC, MGU (3/3)">
			<group id="3000">
				<function start="183" end="183" comment="C_QmaN_Vorhanden - nr001_vorhanden" mask="11111111b">00</function>
				<function start="184" end="187" comment="C_SLA_QmaN_Land_aktiv - FFFFFFFF" mask="11111111b">FA, C3, 81, F8</function>
			</group>	
		</code>	
		<code description="ENABLE Driver Assistant Pro (DAP) - Option to form emergency lane. See BDC, MGU (3/3)">
			<group id="3000">
				<function start="192" end="192" comment="C_RGA_Funktion - Nr001_aktiviert" mask="11111111b">01</function>
				<function start="193" end="196" comment="C_RGA_Land_aktiv - FFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="197" end="200" comment="C_RGA_Seitenwahl_links_Land_aktiv - FFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Driver Assistant Pro (DAP) - Option to form emergency lane. See BDC, MGU (3/3)">
			<group id="3000">
				<function start="192" end="192" comment="C_RGA_Funktion - Nr001_aktiviert" mask="11111111b">00</function>
				<function start="193" end="196" comment="C_RGA_Land_aktiv - FFFFFFFF" mask="11111111b">88, 88, 01, 70</function>
				<function start="197" end="200" comment="C_RGA_Seitenwahl_links_Land_aktiv - FFFFFFFF" mask="11111111b">88, 88, 01, 70</function>
			</group>	
		</code>	
		<code description="ENABLE Driver Assistant Pro (DAP) - Undertaking. See BDC, MGU (3/3)">
			<group id="3001">
				<function start="160" end="160" comment="C_Rechtsueberholen_verbieten - Nr001_aktiviert" mask="11111111b">01</function>
			</group>	
		</code>	
		<code description="DISABLE Driver Assistant Pro (DAP) - Undertaking. See BDC, MGU (3/3)">
			<group id="3001">
				<function start="160" end="160" comment="C_Rechtsueberholen_verbieten - Nr000_deaktiviert" mask="11111111b">00</function>
			</group>	
		</code>	
	</cafd>	
    <cafd id="00003D14" name="DSC_VIP" author="SaNGRia" series="G005, G007, G020, G015, G011">	
		<code description="ENABLE Speed Limit Assist (aSLA). Req ID7 and 11-20 I-Step. See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="111" end="114" comment="C_SLA_aSLA_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="117" end="117" comment="C_SLA_aSLA_vorhanden - Nr001_vorhanden" mask="11111111b">01</function>
				<function start="144" end="144" comment="C_SLA_Anzeige_Zusatztexte - Nr001_aktiviert" mask="11111111b">01</function>
				<function start="210" end="213" comment="C_SLA_Vorausschau_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="215" end="215" comment="C_SLA_Streckenregelung_vorhanden - NR_002_vorhanden_SLA_entkoppelt" mask="11111111b">02</function>
				<function start="216" end="219" comment="C_SLA_Streckenregelung_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Speed Limit Assist (aSLA). See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="111" end="114" comment="C_SLA_aSLA_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">F9, 0F, 86, 00</function>
				<function start="117" end="117" comment="C_SLA_aSLA_vorhanden - Nr001_vorhanden" mask="11111111b">00</function>
				<function start="144" end="144" comment="C_SLA_Anzeige_Zusatztexte - Nr001_aktiviert" mask="11111111b">01</function>
				<function start="210" end="213" comment="C_SLA_Vorausschau_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FB, DF, AF, C0</function>
				<function start="215" end="215" comment="C_SLA_Streckenregelung_vorhanden - NR_002_vorhanden_SLA_entkoppelt" mask="11111111b">00</function>
				<function start="216" end="219" comment="C_SLA_Streckenregelung_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">F9, 0F, 86, 00</function>
			</group>	
		</code>	
		<code description="ENABLE Traffic Light Assistant (TLA). Req ID7, 11-20 I-Step, and aSLA. See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="179" end="182" comment="C_SLA_UCC_Land_aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Traffic Light Assistant (TLA). See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="179" end="182" comment="C_SLA_UCC_Land_aktiv - Nr000_Bausteinpartitionierung" mask="11111111b">00, 00, 00, 00</function>
			</group>	
		</code>	
	</cafd>		
    <cafd id="00003D78" name="DSC_VIP" author="SaNGRia" series="G005, G007, G020">	
		<code description="ENABLE Speed Limit Assist (aSLA). Req ID7 and 11-20 I-Step. See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="111" end="114" comment="C_SLA_aSLA_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="117" end="117" comment="C_SLA_aSLA_vorhanden - Nr001_vorhanden" mask="11111111b">01</function>
				<function start="144" end="144" comment="C_SLA_Anzeige_Zusatztexte - Nr001_aktiviert" mask="11111111b">01</function>
				<function start="210" end="213" comment="C_SLA_Vorausschau_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
				<function start="215" end="215" comment="C_SLA_Streckenregelung_vorhanden - NR_002_vorhanden_SLA_entkoppelt" mask="11111111b">02</function>
				<function start="216" end="219" comment="C_SLA_Streckenregelung_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Speed Limit Assist (aSLA). See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="111" end="114" comment="C_SLA_aSLA_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">F9, 0F, 86, 00</function>
				<function start="117" end="117" comment="C_SLA_aSLA_vorhanden - Nr001_vorhanden" mask="11111111b">00</function>
				<function start="144" end="144" comment="C_SLA_Anzeige_Zusatztexte - Nr001_aktiviert" mask="11111111b">01</function>
				<function start="210" end="213" comment="C_SLA_Vorausschau_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">FB, DF, AF, C0</function>
				<function start="215" end="215" comment="C_SLA_Streckenregelung_vorhanden - NR_002_vorhanden_SLA_entkoppelt" mask="11111111b">00</function>
				<function start="216" end="219" comment="C_SLA_Streckenregelung_Land_Aktiv - 0xFFFFFFFF" mask="11111111b">F9, 0F, 86, 00</function>
			</group>	
		</code>	
		<code description="ENABLE Traffic Light Assistant (TLA). Req ID7, 11-20 I-Step, and aSLA. See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="179" end="182" comment="C_SLA_UCC_Land_aktiv - 0xFFFFFFFF" mask="11111111b">FF, FF, FF, FF</function>
			</group>	
		</code>	
		<code description="DISABLE Traffic Light Assistant (TLA). See 7083, MGU, DSC 3D14 (4/4)">
			<group id="3020">
				<function start="179" end="182" comment="C_SLA_UCC_Land_aktiv - Nr000_Bausteinpartitionierung" mask="11111111b">00, 00, 00, 00</function>
			</group>	
		</code>	
	</cafd>	
</FDL>

