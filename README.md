

#  Car Test
## 1. Project Overview

* This Repo provides an example usage of the Generic Test Trace Framework located in the `Ada_Test_Trace_Framework`

  * Purpose: To test Ada state machine implementations of `Alarm` and `Starter` located in the `Car_Impl_Ada` repo
  * Utilizes generic test framework from `Ada_Trace_Framework`
---


## 2. Setup 

1. **Clone the repository with submodules**

   ```bash
   git clone --recurse-submodules https://github.com/angel-gallegos-1/Car_Test.git
   ```
2. **Build the project**
   ```bash
   gnatmake -P car_test.gpr
   ```
    or
   ```bash
   gprbuild -P car_test.gpr
   ```

3. **Running the Project**
   ```bash
   ./obj/starter_main arg1 arg2
   ./obj/alarm_main arg1 arg2
   ```
- **Two arguments provided**:  
  - `arg1`: Input directory  (kind2 Test Traces directory)
  - `arg2`: Output directory  

- **One argument provided**:  
  - `arg1`: Input directory  (kind2 Test Traces directory)
  - Output directory defaults to `outputs/`

- **No arguments provided**:  
  - User is **prompted** for the input directory 
  - Output directory defaults to `outputs/`
---

