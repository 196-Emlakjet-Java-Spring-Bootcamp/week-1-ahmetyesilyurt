# week-1-ahmetyesilyurt


## **JAVA 11** 

### Running Java Files

 - Java 11 ile beraber tek bir Java dosyasını javac komutu kullanmadan çalıştırabilir hale geldik.
 - JDK java komutu ile çalıştırdığımız bu dosya içerisindeki ilk main metodu bulacak ve eğervarsa verilmiş parametreler ile main metod çalıştırılacaktır.< br >

![javac](https://user-images.githubusercontent.com/44724790/170649756-fb0b4b02-d220-45a7-b59f-079b66dadab3.PNG)

### New String Methods

- **repeat(int)** method
 - int parametresi ile String objesinin kaç defa tekrarlanacağını belirtiyoruz.

![2](https://user-images.githubusercontent.com/44724790/170649968-c17de1a1-acb1-4fec-ae01-98905f1d7861.PNG)

- **isBlank()** method
 -String objesinin boş olması veya sadece whitespace karakter içermesi halinde true dönen bir method.

![3](https://user-images.githubusercontent.com/44724790/170650207-8fd889a1-487f-4497-b201-c25554a7753d.PNG)

- **strip()**, **stripLeading()**, **stripTrailing()** method
 - İlgili String objesi içerisindeki whitespace karakterleri kaldırarak bir String objesi döndürür.
 - **stripLeading()** methodu String objesinin içerisindeki ilk whitespace olmayan karakter öncesindeki whitespace karakterlerini kaldırırken stripTrailing() methoduysa bu işlemi sonrasındaki karakterler için uygular.

![4](https://user-images.githubusercontent.com/44724790/170651628-1fe7d92e-2bd6-45d3-9dbd-f94f9ccd22f7.PNG)

- lines() method
 - Bu methodu ile ilgili String objesinin satırlarını Stream objesi olarak döndürebiliriz. lines() methodunun satır belirlemede kullandığı ifadeler ise şu şekilde : “\n”, “\r”, or “\r\n”.
 
 ![5](https://user-images.githubusercontent.com/44724790/170651744-2113d13a-f314-459a-a6a7-9528c7da5657.PNG)

### Collection
 - toArray(intFunction) Method
 - Koleksiyonları dizilere çevirmek için kullanılan toArray() method eklenmiştir.
![6](https://user-images.githubusercontent.com/44724790/170651936-cc2bef5b-a044-4627-8fb2-5805a2ee4004.PNG)

### Files
 - Dosya okuma ve yazma işlemlerini hızlıca yapmak için readString, writeString metotları eklenmiştir

## **JAVA 17** 

### Restore Always-Strict Floating-Point Semantics
 -  This JEP is mainly for scientific applications, and it makes floating-point operations consistently strict. The default floating-point operations are strict or strictfp, both of which guarantee the same results from the floating-point calculations on every platform.

### Enhanced Pseudo-Random Number Generators
 - Also related to more special use cases, JEP 356 provides new interfaces and implementations for Pseudo-Random Number Generators (PRNG).So, it's easier to use different algorithms interchangeably, and it also offers better support for stream-based programming:

### New macOS Rendering Pipeline
 - This JEP implements a Java 2D internal rendering pipeline for macOS since Apple deprecated the OpenGL API (in macOS 10.14), used internally in Swing GUI. The new implementation uses the Apple Metal API, and apart from the internal engine, there were no changes to the existing APIs.
 
###  Deprecate the Applet API for Removal
 - Although this may be sad for many Java developers who started their development career using Applet APIs, many web browsers have already removed their support for Java plugins. As the API became irrelevant, this version marked it for removal even though it has been marked as deprecated since version 9.
 
###  Pattern Matching for Switch 
 - This is another step toward pattern matching by enhancing pattern matching for switch expressions and statements. It reduces the boilerplate necessary to define those expressions and improves the expressiveness of the language.
 
![11](https://user-images.githubusercontent.com/44724790/170652429-6d974cd6-c3a3-4fd7-9261-4418953be792.PNG)

### Sealed Classes
 -  Sealed classes are part of Project Amber, and this JEP officially introduces a new feature to the language, although it was available in preview mode in the JDK versions 15 and 16.The feature restricts which other classes or interfaces may extend or implement a sealed component. Showing another improvement related to pattern matching combined with the JEP 406 will allow a more sophisticated and cleaner inspection of the type, cast and act code pattern.
 
![12](https://user-images.githubusercontent.com/44724790/170652481-3b9ad227-453c-41ac-a83c-4b7ef9e10c6b.PNG)

### Vector API (Second Incubator) 
- The Vector API deals with the SIMD (Single Instruction, Multiple Data) type of operation, meaning various sets of instructions executed in parallel. It leverages specialized CPU hardware that supports vector instructions and allows the execution of such instructions as pipelines.As a result, the new API will enable developers to implement more efficient code, leveraging the potential of the underlying hardware.

 ![13](https://user-images.githubusercontent.com/44724790/170652973-88c2b7d2-2d5a-4f72-a69f-5e4293aa54a9.PNG)

