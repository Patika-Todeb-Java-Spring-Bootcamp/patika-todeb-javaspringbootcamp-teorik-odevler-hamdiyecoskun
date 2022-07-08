patika-todeb-javaspringbootcamp-teorik-odevler-hamdiyecoskun
patika-todeb-javaspringbootcamp-teorik-odevler-hamdiyecoskun created by GitHub Classroom
## 1 – IOC and DI means ?
 
`Inversion of control` bir yazılım tasarım prensibidir. IOC ile uygulama içerisindeki obje instance’larının yönetimi sağlanarak, bağımlılıklarını en aza indirgemek amaçlanmaktadır. Projemizdeki bağımlılıkların oluşturulmasını ve yönetilmesini geliştiricinin yerine, framework’ün yapması olarak da açıklanabilir.

Bağımlılık oluşturacak nesneleri direkt olarak kullanmak yerine, bu nesnelerin dışardan verilmesiyle sistem içerisindeki bağımlılığı minimize etmek amaçlanır. Böylece bağımlılık bulunan sınıf üzerindeki değişikliklerden korunmuş oluruz.
`Dependency injection` bir sınıfın/nesnenin bağımlılıklardan kurtulmasını amaçlayan ve o nesneyi olabildiğince bağımsızlaştıran bir programlama tekniği/prensibidir.
## 2 – Spring Bean Scopes ?
### Bean Nedir ?
Spring Framework uygulamamızın omurgasını oluşturan ve Spring IOC container tarafından yönetilen nesnelere `BEAN` denir. Yeniden kullanılabilir objeler olarak kabul edebiliriz.
### Scope Nedir ?
`Scope` kelimesi kapsam, alan, faaliyet alanı gibi anlamlar taşımakta biz de Bean objelerimizin birer yaşam alanının var olduğunu düşünebiliriz.

### Scope Türleri
- `Singleton` : Her Bean varsayılan olarak singleton olmakla birlikte sadece bir kez üretilir. Singleton Design Pattern’deki gibi düşünebiliriz. Bir kere üret tekrar tekrar kullan.
- `Prototype` : Söz konusu olan bean için her bir istek yapıldığında oluşturulur. Her oluşturmada farklı bir instance üretilir.
- `Request` : Request bean’i adından da yola çıkarak HTTP isteği geldiğinde oluşturulur. HTTP request düzeyinde etkin bir şekil kapsama alınır.
- `Session` : Session Scope Web Uygulamalarında HTTP isteği geldiğinde oluşturulur. Request Scope’a benzer bir yaklaşım.
- `Global Session` : Bir HTTP’nin yaşam döngüsünde tek bir Bean’ın tanımını kapsamaktadır. Yanlızca WEB’e duyarlı bir Spring’te geçerlidir.
## 3 – What does @SpringBootApplication do ?
`@SpringBootApplication` anotasyonu uygulamanın giriş metodunu belirtir. Yani halk arasındaki tabir ile main fonksiyondur. Uygulama bu metod ile başlar.
`@SpringBootApplication`, sınıfın bir yapılandırma sınıfı olduğunu, `@EnableAutoConfiguration` ve bileşende `@ComponentScan` açıklaması aracılığıyla tarama yoluyla otomatik yapılandırmayı tetiklediğini belirtir. Spring Uygulama Bağlamının otomatik yapılandırmasını sağlar.
## 4 – Why Spring Boot over Spring?
`Spring Boot` `Spring Framework`’e hızlı uygulama geliştirme özelliği sağlayan bir spring modülüdür.
Basit ve web tabanlı uygulamaları kurmak, yapılandırmak ve çalıştırmak için daha kolay ve hızlı bir yol sağlar. XML yapılandırması için gereklilik yoktur. Gömülü http sunucuları yardımıyla web uygulamalarını kolayca test eder.
## 5 – What is Singleton and where to use it ?
`Singleton`(tek nesne) tasarım kalıbı, bir sınıfın tek bir örneğini almak için kullanılır. Veritabanı bağlantısı, ön-bellek , yapılandırma dosyası gibi uygulamalarda kullanılır.
## 6 – Explain @RestController annotation in Sprint boot?
`@RestController` URL ile istenen request’lere ait dönüş biçiminde herhangi bir template engine'ne (şablon motoru) ihtiyaç duymaz. Datanın kendisini JSON veya XML formatı ile direkt olarak sunar.
## 7 - What is the primary difference between Spring and Spring Boot ?
`Spring Boot` `Spring framework`’e hızlı uygulama geliştirme (RAD) özelliği sağlayan bir spring modülüdür.`Spring boot` içerisinde gömülü http serverları barındırır. Xml konfigürasyonunu otomatikleştirir.

