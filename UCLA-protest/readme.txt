** UCLA PROTEST IMAGE DATASET


- Documented on 12/12/2017 by Jungseock Joo (jjoo@comm.ucla.edu)
- This dataset can be used for academic purpose only. 
- We do not own the copyrights of any photographs. The photographs may be copyright-protected. 
- https://arxiv.org/pdf/1709.06204.pdf
- If you use this dataset in your work, please cite the following paper: 


Donghyeon Won, Zachary C. Steinert-Threlkeld, and Jungseock Joo. 2017. Protest Activity Detection and Perceived Violence Estimation from Social Media Images. In Proceedings of the 25th ACM International Conference on Multimedia. ACM, 786-794.


@inproceedings{won2017protest,
 title={Protest Activity Detection and Perceived Violence Estimation from Social Media Images},
 author={Won, Donghyeon and Steinert-Threlkeld, Zachary C and Joo, Jungseock},
 booktitle = {Proceedings of the 25th ACM International Conference on Multimedia},
  pages={786--794},
  organization = {ACM}
  year={2017}
}


* Data format
annot_train.txt 
annot_test.txt
<image file name #1> <protest> <violence> <sign> <photo> <fire> <police> <children> <group_20> <group_100> <flag> <night> <shouting>
<image file name #2> <protest> <violence> <sign> <photo> <fire> <police> <children> <group_20> <group_100> <flag> <night> <shouting>
...


- <protest> contains a binary value: 1 (protest) or 0 (not protest)
- <violence> contains a real number in range between 0 (least violent) and 1 (most violent) or “-” (not applicable, i.e., not a protest image)
- Other visual attributes are all binary: 1 (with the attribute), 0 (without the attribute), or “-” (not applicable, i.e., not a protest image)
- Please note that only protest images (images for which <protest> = 1) have violence and visual attribute annotations.