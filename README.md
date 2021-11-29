###**Αρχιτεκτονική Προηγμένων Υπολογιστών**
1. CPU: minor
   _Από το starter-se.py:_  
   CPU frequency: 1GHz  
   Number of CPU cores: 1  
   Type of memory to use: DDR3-1600-8x8  
   Number of memory channels: 2  
   Number of memory ranks per channel: None  
   Physical memory size: 2GB  


2. sim-seconds    0.000035                       # Number of seconds simulated  
   sim-insts                                        5027                       # Number of instructions simulated  
   host-inst-rate                                  80811                       # Simulator instruction rate (inst/s)  


3. Total-Inst-num=5027  
   All misses were 0 (???)  
   CPI=1  
   

4. Τα μοντέλα in-order CPUs είναι:  
* **SimpleCPU:** Πρόκειται για ένα απλό μοντέλο που χρησιμοποιείται για απλές, μη απαιτητικές περιπτώσεις και διαχωρίζεται σσε 3 είδη:  
  * _BaseSimpleCPU:_ Δεν χρησιμοποιείται από μόνο του, αλλά κληρονομεί κάποια classes από τα άλλα δύο είδη. 
  * _AtomicSimpleCPU:_ Χρησιμοποιεί atomic memory accesses. Είναι αρκετά γρήγορο στο readMem & writeMem.
  * _TimingSimpleCPU:_ Είνια πιο περίπλοκο. Η εκτέλεση των εντολών χρειάζεται περισσότερο χρόνο.
* **Minor:** Έχει ορισμένο pipeline, αλλά προσαρμόσιμα data structures και τρόπο εκτέλεσης.  
  





##_**Πηγές**_
[CPU models](https://www.gem5.org/documentation/general_docs/cpu_models/SimpleCPU)

_**Σημείωση:** Έχω αντικαταστήσει την κάτω παύλα με κανονική._
