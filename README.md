## EricssonKPI
Gathering Ericsson KPIs (LTE, VoLTE, RSSI) via Amos language

## Example for collecting KPIs by using EricssonAmosFormulasbyEUlusoy.txt (This file should be located under /home/shared/$username1/)
uv sls_username > $username1 
pmxhe . ^Acc_ErabAttempt$|^Acc_InitialERabEstabSuccRate$|^Acc_InitialERabEstabFailCount$|^Acc_InitialERabEstabSuccRateQci1$|^Acc_InitialERabEstabFailCountQci1$|^Ret_ERabRetainabilityRate$|^Ret_ERabRetainabilityCount$|^Ret_ERabRetainabilityRateQci1$|^Ret_ERabRetainabilityCountQci1$|^Mob_IRAT_Redirect$|^CSFB$|^DL_VOL$|^Int_DlThroughput_kbps$|^UL_VOL$|^Int_UlThroughput_kbps$|^Tot_Downtime$ -f /home/shared/$username1/EricssonAmosFormulasbyEUlusoy.txt  -tz -7 -o csv  -m 48 -h
