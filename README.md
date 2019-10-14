# MOMICE
Public version of the MOMICE gas-grain astrochemical code

MOMICE is a gas-grain astrochemical model that computes the temporal evolution of the chemical composition in the gas phase and on the interstellar grain surfaces. The approach is based on the rate equations introduced by Hasegawa et al. (1992) for a gas-grain treatment and allows you to follow the chemistry with fixed or evolving physical conditions. Among others, two of the main specifications of MOMICE is the multiphase treatment for the formation and desorption of ices and the computation of the reaction probabilities of grain surface reactions with the Eckart model from quantum chemical calculations. MOMICE is based on the GRAINOBLE code developed at IPAG between 2009 and 2012, and further modified and updated between 2013 and 2019. 

The MOMICE code, written in Fortran90, comes with two Python routines to run and analyse the simulations. MOMAPP (MOMice APPlier) allows you to execute MOMICE for 1) individual simulations with constant physical conditions, 2) simulations for evolving physical conditions as function of distance, 3) model grids in which physical conditions are explored, 4) sensitivity analyses in which the distributions of key input parameters impacts the uncertainties of the model predictions. MOMAN (MOMice ANalyser) allows you to read the binary files generated by GRAINOBLE and visualise the results via different kinds of figures. 

For a full description of the physical and chemical processes included in the model and for some results, please take a look at my thesis manuscript, available [here](http://tel.archives-ouvertes.fr/tel-00790641), and the publications listed below.

The `instructions` file describes the input files needed by MOMICE, how to compile and execute the code, and the routines needed to analyze and visualise the results. The `log_history` file gives an overview of all previous versions of the code between 2012 and 2018. 

### Publications: 

F. Dulieu, T. Nguyen, E. Congiu, S. Baouche, V. Taquet 2019, *Efficient formation route of the pre-biotic molecule formamide on interstellar dust grains*, **MNRAS**, L119 ([URL](https://academic.oup.com/mnrasl/article/484/1/L119/5305861))

V. Taquet, K. Furuya, C. Walsh, E. F. van Dishoeck 2016, *A primordial origin for molecular oxygen in comets: A chemical
  kinetics study of the formation and survival of O2 ice from clouds to disks*, **MNRAS**, 462, 99 ([URL](http://mnras.oxfordjournals.org/content/462/Suppl_1/S99))
  
V. Taquet, E. Wirstrom, S. B. Charnley 2016, *Formation and recondensation of complex organic molecules during 
  protostellar luminosity outbursts*, **ApJ**, 821, 46 ([URL](http://iopscience.iop.org/article/10.3847/0004-637X/821/1/46/meta))
  
V. Taquet, S. B. Charnley, O. Sipilä 2014, *Multilayer Formation and Evaporation of Deuterated Ices in
  Prestellar and Protostellar Cores*, **ApJ**, 791, 1 ([URL](https://iopscience.iop.org/article/10.1088/0004-637X/791/1/1))
  
V. Taquet, P. Peters, C. Kahane, C. Ceccarelli, D. Duflot, C. Toubin, A. Faure, L. Wiesenfeld 2013, *Modelling of deuterated water ice formation*, **A&A**, 550, A127 ([URL](http://www.aanda.org/articles/aa/abs/2013/02/aa20084-12/aa20084-12.html))

V. Taquet, C. Ceccarelli, C. Kahane 2012, *Formaldehyde and methanol deuteration in protostars: fossiles from a
  past fast high density pre-collapse phase*, **ApJL**, 748, L3 ([URL](http://iopscience.iop.org/2041-8205/748/1/L3?fromSearchPage=true))
  
V. Taquet, C. Ceccarelli, C. Kahane 2012, *Multilayer modeling of grain porous surface chemistry I. The
  GRAINOBLE code*, **AA**, 538, 42 ([URL](http://www.aanda.org/index.php?option=com_article&access=standard&Itemid=129&url=/articles/aa/full_html/2012/02/aa17802-11/aa17802-11.html))
  
### Acknowledgments 

I would like to thank the following people who helped me developing the model over the years: Cecilia Ceccarelli, Claudine Kahane, Philip Peters, Steve Charnley, Kenji Furuya, Franck Hersant, and Mathieu Van der Swaelmen. 

