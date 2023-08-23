This analysis has 4 steps. In this directory are job submission scripts to condor.

Step 1 is reconstruction -  This is not being redone so there are no scripts for this steps. The output directory of step1 files are stored in /data/user/tmcelroy/domeff/hd5/effxredo/(simulation) and /data/user/tmcelroy/domeff/datahd5/

Step 2 is where most of the dom and event cuts happen - run_ProcessDomInfo_eff100_sim.submit and run_ProcessDomInfo_eff100_sim.sh files are used. Use this as the basis for other efficiencies(90, 110, 120) as well.

Step 3 calculates the weighted avergae charge for every 20 m distance bins - No submission script required - python ComputeChargeDist.py -d /data/user/akatil/domeff/final_aug22/220_cut/dust_layer_correction/datahd5/ -o /data/user/akatil/domeff/final_aug22/220_cut/dust_layer_correction/ComputeCharge/data_chargeDist

Step 4 does not require a submission script. 
