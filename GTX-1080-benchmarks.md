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

2. GoogleNet
    * forward: 105ms (-30ms, -22%)
    * for+back: 342ms (-103ms, -23%)

3. Overfeat
   * forward: 69ms (-21ms, -23%)
   * for+back: 232ms (-47ms, -16%)

4. VGG (OxfordNet)
   * forward: 124ms (-34ms, -21%)
   * for+back: 394ms (-146ms, -27%)
