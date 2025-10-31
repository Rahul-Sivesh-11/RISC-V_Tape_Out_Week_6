# Inception of open-source EDA, OpenLANE and Sky130 PDK



```bash
cd~/Desktop/work/tools/openlane_working_dir/openlane
```
 **Building PDKs from Source**

```bash
export PDK_ROOT=/home/vsduser/Desktop/work/tools/openlane_working_dir/pdks
cd ~/Desktop/work/tools/openlane_working_dir/openlane
alias docker='docker run -it -v $(pwd):/openLANE_flow -v $PDK_ROOT:$PDK_ROOT -e PDK_ROOT=$PDK_ROOT -u $(id -u $USER):$(id -g $USER) efabless/openlane:v0.21'
docker
./flow.tcl -interactive
```

<img width="737" height="519" alt="Screenshot 2025-10-31 151619" src="https://github.com/user-attachments/assets/4ea1f888-baaf-4eb5-af54-aa7daa8a8676" />


```bash
package require openlane 0.9
```

```bash
prep -design picorv32a
```
<img width="1217" height="568" alt="Screenshot 2025-10-31 155819" src="https://github.com/user-attachments/assets/def0457b-fce4-42e0-bc0a-d746e7db9e37" />

```bash
run_synthesis
```

<img width="735" height="518" alt="Screenshot 2025-10-31 152005" src="https://github.com/user-attachments/assets/19640a70-2ebe-4864-8565-c99e734d7d19" />




