Open Babel
----------

Open Babel is a chemical toolbox designed to speak the many languages
of chemical data. It's an open, collaborative project allowing anyone
to search, convert, analyze, or store data from molecular modeling,
chemistry, solid-state materials, biochemistry, or related areas. 

For more information about Open Babel, check the [Open Babel website](http://openbabel.org/).

This is a fork of the [Open Babel project](https://github.com/openbabel/openbabel), optimized for parallelization of 
compound processing in ACGui. To successfully compile the project, please follow the instructions below: 
```
git clone https://github.com/miemiemmmm/openbabel.git
cd openbabel && mkdir build && cd build 
# Replace here with the desired path for installation and python executable
cmake -DRUN_SWIG=ON -DCMAKE_INSTALL_PREFIX=%INSTALLATION_PATH% -DPYTHON_BINDINGS=ON -DPYTHON_EXECUTABLE:FILEPATH=%PYTHON_EXECUTABLE% -DCMAKE_EXPORT_COMPILE_COMMANDS=ON ../; 
make -j8 VERBOSE=1; 
make test; 
make install
```




