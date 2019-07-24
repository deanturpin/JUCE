# Dependencies
```bash
sudo apt install -y \
libfreetype6-dev \
libxinerama-dev \
webkit2gtk-4.0
```

# Configure
```bash
git clone --depth=1 https://github.com/WeAreROLI/JUCE
cd JUCE/extras/Projucer/Builds/LinuxMakefile
```

# Change this flag so you can run without a Roli account
../../JuceLibraryCode/AppConfig.h
```c++
#ifndef JUCER_ENABLE_GPL_MODE
 #define JUCER_ENABLE_GPL_MODE 1
#endif
```

```bash
make -j $(nproc)
```

# Run Projucer
```bash
build/Projucer
```
