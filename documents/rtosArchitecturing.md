
## Creating FreeRTOS Architecture Diagrams ##

I typically create one overall interaction diagram showing each “execution unit” 
(a Task, ISR, Timer Call back, or driver subroutine), each Hardware device, each major datastore, and each major queue/semaphore/mutex with arrow showing their interrelationships. For example, if an ISR triggers a driver task with a semaphore, the Device symbol will point to the ISR with an interrupt arrow, the ISR to the semaphore, the semaphore to the driver task and the driver task to the device. The driver will also have any arrows needed to indicate what it does with the results from the device. I then document the flow of each task individually (with links out representing these interactions)



- https://www.geeksforgeeks.org/system-design/unified-modeling-language-uml-sequence-diagrams/#what-are-sequence-diagrams

https://plantumleditor.com/webedit/?source=dP8zJiD048NxFSNW2gnGG6cXA18KAIZuAMZSBFR4NX7lBBlZ10NbH1o1BYTZOZksaHj4OtlVqxxtpSYBmDfpNQtLcVEwg3GmqWxOrwYK4yjancdB4Dq4iyFawdf--68TtWxVgOtZ9ypGRD37SMgNfYZXmHkAG0VmdQFUQwmHeiVZgt4QuG_PpsZpDlcUjaDmQ6IbTCPcenc7fZMHKvP48ZdsUW8lsZ2io8E62aFG1G8Jl68gIOw2OSp1M96un0xlqqdDli-0otbhG097v_n2vJWbKEMqVjOHoyrRiemV365hE2j78tGpDPUzh961LfsOm5tBEC2dTW9BWVUddZ6gwBzHJzlx9sW_wNWn_NS26TbGLoYT4gNKGfxoR_q0



## Beyond RTOS

https://www.youtube.com/playlist?list=PLPW8O6W-1chytjkg63-tM7MI0BvGxxPIP

