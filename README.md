## About

This is a clever parallel threading benchmark written by [John Tsiombikas](https://github.com/jtsiomb) in 2006 and released under the GPL v 2. It renders a scene, creating a bitmap image. Ian Mapleson has been charting the speed of [different computers on this benchmark](http://www.sgidepot.co.uk/c-ray.html) for many years. This simple program compiles on many computer architectures, allowing you to see how a recent (as of 2022) [Intel Alderlake or Apple M1 Pro](https://github.com/neurolabusc/AppleSiliconForNeuroimaging) compares to a vintage [Silicon Graphics 32 core](http://www.sgidepot.co.uk/c-ray.html) computer. The rendering is an [embarrassingly_parallel](https://en.wikipedia.org/wiki/Embarrassingly_parallel) task, so it performs dramatically faster with multiple threads. The included text file `README.txt` includes additional details.

![Rendered scene](scene.jpg)

Running the benchmark should be simple for most Linux computers with a c compiler installed:

```
git clone https://github.com/neurolabusc/c-ray.git
cd c-ray
make
./RUN.full
```

