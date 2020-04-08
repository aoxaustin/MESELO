# MESELO
 Online Frequent Episode Mining  

MESELO algorithm manuals:  

algorithm parameters:  
/**  
	 * @param inputFile  
	 *            - input event sequence dataset.  
	 * @param outputFile  
	 *            - output frequent episode by each time slot.  
	 * @param min_sup  
	 *            - minimal support threshold.  
	 * @param delta  
	 *            - maximal occurrence window threshold.  
	 * @param window_size  
	 *            - window size for valid sequence.  
	 * @param updateFrequency  
	 *            - when time slot is bigger than DELTA, the algorithm will  
	 *            output frequent episodes every updateFrequency.  
	 * @param begin  
	 *            - begin time slot on the sequence.  
	 * @param end  
	 *            - end time slot on the sequence. for whole sequence to test,  
	 *            begin = 1, end = |event sequence|.  
	 */
	 
e.g. 
 java -jar MESELO.jar ./data/alginput/synthetic/toy2sequence.dat ./data/freqepisodes/synthetic/toy2sequence.csv 2 3 6 2 1 8  

MEANS  
  inputFile = "./data/alginput/synthetic/toy2sequence.dat"  
  ouputFile = "./data/freqepisodes/synthetic/toy2sequence.csv"  
  minimal support = 2  
  maximal occurrence window = 3  
  window size of valid seqeunce = 6  
  updateFrequency = 2  
  begin time slot = 1  
  end time slot = 8, which is the sequence length here.  

The running example data is located at ./data/alginput/synthetic/toy2sequence.dat  

The stock data used in paper is located at ./data/alginput/real/chinaStock/stock-1(to 6).data  

Database structure, just import ./node.sql to MySQL database.  

## Paper info:

[Xiang Ao, Ping Luo, Chengkai Li, Fuzhen Zhuang, Qing He. Online Frequent Episode Mining. In Proceedings of the 31st IEEE International Conference on Data Engineering (ICDE 2015).](https://ieeexplore.ieee.org/document/7113342)

## Bibtex:
`
@inproceedings{ao2015online,  
  title={Online frequent episode mining},  
  author={Ao, Xiang and Luo, Ping and Li, Chengkai and Zhuang, Fuzhen and He, Qing},  
  booktitle={2015 IEEE 31st International Conference on Data Engineering},  
  pages={891--902},  
  year={2015},  
  organization={IEEE}  
}
`
