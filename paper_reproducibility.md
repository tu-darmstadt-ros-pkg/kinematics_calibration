<!-- Panda 1-->
python3 generate_complete_analysis.py --model panda --data panda_1/front_center
<!-- Panda 2-->
python3 generate_complete_analysis.py --model panda --data panda_2/frontcenter
<!--  Panda 3-->
python3 generate_complete_analysis.py --model panda --data panda_3/front
<!--  FR3 -->
python3 generate_complete_analysis.py --model panda --data fr3/front
<!--  Kuka 14 -->
python3 generate_complete_analysis.py --model iiwa14 --data kuka_14/front
<!--  Kinova -->
python3 generate_complete_analysis.py --model gen3lite --data kinova/front --repeatability 1

<!-- Bar plot -->
python3 statistical_analysis_many_to_one.py --model panda --data panda_2_bis/left panda_2_bis/front panda_2_bis/right-high

<!--Comparison and Ablation study-->
python3 comparison_with_sota.py --model panda --data panda_1/front_center 
<!-- Extra Bar plot -->

python3 statistical_analysis_many_to_one.py --model gen3lite --data dinova_2/front dinova_2/left dinova_2/right-high -pnm

python3 statistical_analysis_many_to_one.py --model iiwa14 --data kuka_14/front kuka_14/left_back kuka_14/raised_left -pnm

python3 statistical_analysis_many_to_one.py --model panda --data panda_2/back_left panda_2/back_right panda_2/front_center panda_2/front_left panda_2/front_right panda_2/high panda_2/mid_left panda_2/mid_right panda_2/mid-high

python3 statistical_analysis_many_to_one.py --model panda --data panda_2_clean/back_left panda_2_clean/back_right panda_2_clean/front_center panda_2_clean/front_left panda_2_clean/front_right panda_2_clean/mid_left panda_2_clean/mid_right panda_2_clean/mid-high

python3 statistical_analysis_many_to_one.py --model panda --data panda_4/front  panda_4/right panda_4/very-front

python3 statistical_analysis_many_to_one.py --model panda --data panda_6/front panda_6/left panda_6/right