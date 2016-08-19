# Benchmarks of GTX 1080

Hardware:
* Zotac GTX 1080 AMP!
* CPU: i5-6600 3.5GHz

Software:
* Ubuntu 16.04
* CUDA 8 RC
* TensorFlow 0.10rc

Benchmarked with https://github.com/soumith/convnet-benchmarks

In original benchmark, Titan X was used. In numbers below, I put delta from it's values in brackets.

## Tensorflow 0.10rc

1. AlexNet:
    * forward: 22ms (-4ms, -15%)
    * for+back: 68ms (-13ms, -16%)
    * CPU forward: 1815ms (82.5x slower)
    * CPU for+back: 5542ms (81.5x slower)

2. GoogleNet
    * forward: 105ms (-30ms, -22%)
    * for+back: 342ms (-103ms, -23%)
    * CPU forward: 4458ms (42.5x slower)
    * CPU for+back: 15012ms (43.8x slower)

3. Overfeat
   * forward: 69ms (-21ms, -23%)
   * for+back: 232ms (-47ms, -16%)
   * CPU forward: 6281ms (91x slower)
   * CPU for+back: 20342ms (87.6x slower)

4. VGG (OxfordNet)
   * forward: 124ms (-34ms, -21%)
   * for+back: 394ms (-146ms, -27%)
   * CPU forward: 9192ms (74x slower)
   * CPU for+back: 28630ms (72.6x slower)
