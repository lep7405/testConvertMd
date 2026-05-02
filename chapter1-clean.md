# Chapter 1

## Introduction

The Spring framework (shortly, Spring) is an application framework that is part of the Java ecosystem.
(Spring framework (viết tắt là Spring) là một framework ứng dụng nằm trong hệ sinh thái Java.)

An application framework is a set of common software functionalities that provides a foundation structure for developing an application.
(Khung ứng dụng là một tập hợp các chức năng phần mềm phổ biến cung cấp cấu trúc nền tảng để phát triển ứng dụng.)

An application framework eases the effort of writing an application by taking out the effort of writing all the program code from scratch.
(Khung ứng dụng giúp giảm bớt nỗ lực viết ứng dụng bằng cách loại bỏ nỗ lực viết tất cả mã chương trình từ đầu.)

We use Spring in the development of many kinds of applications nowadays, from large backend solutions to automation testing apps.
(Hiện nay, chúng tôi sử dụng Spring để phát triển nhiều loại ứng dụng, từ các giải pháp phụ trợ lớn đến các ứng dụng thử nghiệm tự động hóa.)

According to many survey reports on Java technologies (like this one of JRebel from 2020: http:// mng.bz/N4V7; or this one from JAXEnter: http://mng.bz/DK9a), Spring is the most used Java framework today.
(Theo nhiều báo cáo khảo sát về công nghệ Java (như báo cáo này của JRebel từ năm 2020: http:// mng.bz/N4V7; hoặc báo cáo này của JAXEnter: http://mng.bz/DK9a), Spring là framework Java được sử dụng nhiều nhất hiện nay.)

Spring is popular, and developers have started to use it more often with other JVM languages than Java as well.
(Spring rất phổ biến và các nhà phát triển cũng bắt đầu sử dụng nó thường xuyên hơn với các ngôn ngữ JVM khác ngoài Java.)

In the last few years, we observed an impressive
(Trong vài năm qua, chúng tôi đã quan sát thấy một sự ấn tượng)

growth of developers using Spring with Kotlin (another appreciated language from the JVM family).
(sự phát triển của các nhà phát triển sử dụng Spring với Kotlin (một ngôn ngữ được đánh giá cao khác từ dòng JVM).)

In this book, we’ll focus on the foundations of Spring, and I’ll teach you essential skills for using Spring in real-world examples.
(Trong cuốn sách này, chúng tôi sẽ tập trung vào nền tảng của Spring và tôi sẽ dạy bạn những kỹ năng cần thiết để sử dụng Spring trong các ví dụ thực tế.)

To make the subject more comfortable for you and allow you to focus on Spring, we’ll use only Java examples.
(Để giúp bạn thoải mái hơn với chủ đề này và cho phép bạn tập trung vào Spring, chúng tôi sẽ chỉ sử dụng các ví dụ về Java.)

Throughout the book, we’ll discuss and apply, with examples, essential skills like con-necting to a database, establishing communication between applications, and secur-ing and testing an app.
(Xuyên suốt cuốn sách, chúng ta sẽ thảo luận và áp dụng, kèm theo các ví dụ, các kỹ năng cần thiết như kết nối với cơ sở dữ liệu, thiết lập liên lạc giữa các ứng dụng cũng như bảo mật và thử nghiệm một ứng dụng.)

Before diving into more technical details in the next chapters, let’s talk about the Spring framework and where you’ll actually use it.
(Trước khi đi sâu vào chi tiết kỹ thuật hơn trong các chương tiếp theo, hãy nói về Spring framework và nơi bạn sẽ thực sự sử dụng nó.)

Why is Spring so appreciated, and when should you even use it?
(Tại sao Spring lại được đánh giá cao như vậy và khi nào bạn nên sử dụng nó?)

In this chapter, we’ll focus on what a framework is, referring in particular to the Spring framework.
(Trong chương này, chúng ta sẽ tập trung vào framework là gì, đặc biệt đề cập đến Spring framework.)

In section 1.1, we discuss the advantages of using a framework.
(Trong phần 1.1, chúng ta thảo luận về những lợi ích của việc sử dụng một framework công tác.)

In section 1.2, we discuss the Spring ecosystem with the components you need to learn to get started with Spring.
(Trong phần 1.2, chúng ta thảo luận về hệ sinh thái Spring với các thành phần bạn cần tìm hiểu để bắt đầu với Spring.)

Then I’ll take you through possible usages of the Spring framework—in particular, real-world scenarios in section 1.3.
(Sau đó, tôi sẽ hướng dẫn bạn các cách sử dụng có thể có của Spring framework—đặc biệt là các tình huống trong thế giới thực trong phần 1.3.)

In section 1.4, we’ll dis-cuss when using frameworks might not be the right approach.
(Trong phần 1.4, chúng ta sẽ thảo luận khi nào việc sử dụng các framework có thể không phải là phương pháp phù hợp.)

You need to under-stand all these things about the Spring framework before trying to use it.
(Bạn cần hiểu tất cả những điều này về Spring framework trước khi thử sử dụng nó.)

Otherwise, you might try to use a hammer to dig your garden.
(Nếu không, bạn có thể thử dùng búa để đào khu vườn của mình.)

Depending on your level, you might feel this chapter difficult.
(Tùy thuộc vào trình độ của bạn, bạn có thể cảm thấy chương này khó khăn.)

I might introduce some notions that you haven’t heard about, and this aspect might disturb you.
(Tôi có thể giới thiệu một số khái niệm mà bạn chưa từng nghe đến và khía cạnh này có thể làm phiền bạn.)

But don’t worry; even if you don’t understand some of the things now, they will be clarified later in the book.
(Nhưng đừng lo lắng; ngay cả khi bây giờ bạn không hiểu một số điều, chúng sẽ được làm rõ sau trong cuốn sách.)

Sometimes, throughout the book, I’ll refer to something said in earlier chapters.
(Đôi khi, xuyên suốt cuốn sách, tôi sẽ đề cập đến những điều đã nói ở các chương trước.)

I use this approach because learning a framework like Spring doesn’t always offer us a linear learning path, and sometimes you need to wait until you get more pieces of the puzzle before you see the complete picture.
(Tôi sử dụng phương pháp này vì việc học một khuôn khổ như Spring không phải lúc nào cũng cung cấp cho chúng ta một lộ trình học tập tuyến tính và đôi khi bạn cần đợi cho đến khi có được nhiều mảnh ghép hơn trước khi bạn nhìn thấy bức tranh hoàn chỉnh.)

But in the end, you’ll get a clear image, and you’ll get the valuable skills you need to develop apps like a professional.
(Nhưng cuối cùng, bạn sẽ có được một hình ảnh rõ ràng và bạn sẽ có được những kỹ năng quý giá cần thiết để phát triển ứng dụng như một người chuyên nghiệp.)

## Why Should We Use Frameworks?

In this section, we discuss frameworks.
(Trong phần này, chúng ta thảo luận về các framework.)

What are they?
(Họ là gì?)

How did this concept appear, and why?
(Khái niệm này xuất hiện như thế nào và tại sao?)

To be motivated to use something, you need to know how that something brings you value.
(Để có động lực sử dụng thứ gì đó, bạn cần biết thứ đó mang lại giá trị cho bạn như thế nào.)

And that’s also the case with Spring.
(Và đó cũng là trường hợp của Spring.)

I’ll teach you these essential details by sharing the knowledge I gathered from my own experience and by studying and using various frameworks in real-world scenarios, including Spring.
(Tôi sẽ dạy cho bạn những chi tiết cần thiết này bằng cách chia sẻ kiến ​​thức tôi thu thập được từ kinh nghiệm của bản thân cũng như bằng cách nghiên cứu và sử dụng các framework khác nhau trong các tình huống thực tế, bao gồm cả Spring.)

An application framework is a set of functionalities on top of which we build appli-cations.
(Khung ứng dụng là một tập hợp các chức năng mà trên đó chúng ta xây dựng các ứng dụng.)

The application framework provides us a broad set of tools and functionalities that you can use to build apps.
(Khung ứng dụng cung cấp cho chúng tôi một bộ công cụ và chức năng phong phú mà bạn có thể sử dụng để xây dựng ứng dụng.)

You don’t need to use all the features the framework offers.
(Bạn không cần phải sử dụng tất cả các tính năng mà framework cung cấp.)

Depending on the requirements of the app you make, you’ll choose the right parts of the framework to use.
(Tùy thuộc vào yêu cầu của ứng dụng bạn tạo, bạn sẽ chọn phần phù hợp của framework để sử dụng.)

Here’s an analogy I like for application frameworks.
(Đây là một sự tương tự mà tôi thích đối với các framework ứng dụng.)

Did you ever buy a piece of furniture from a DIY store like Ikea?
(Bạn đã bao giờ mua một món đồ nội thất từ ​​cửa hàng DIY như Ikea chưa?)

Say you buy a wardrobe—you won’t get an assem-bled wardrobe, but the right components you need to build it and a manual on how to assemble your piece of furniture.
(Giả sử bạn mua một chiếc tủ quần áo—bạn sẽ không nhận được một chiếc tủ quần áo lắp ráp nhưng bạn cần có những bộ phận phù hợp để tạo nên tủ và sách hướng dẫn cách lắp ráp đồ nội thất của mình.)

Now imagine you ordered a wardrobe, but instead
(Bây giờ hãy tưởng tượng bạn đặt mua một chiếc tủ quần áo, nhưng thay vào đó)

of getting only the right components you need, you get all the possible components you can use to assemble any piece of furniture: a table, a wardrobe, and so on.
(Để chỉ lấy đúng các thành phần bạn cần, bạn sẽ có được tất cả các thành phần có thể sử dụng để lắp ráp bất kỳ món đồ nội thất nào: bàn, tủ quần áo, v.v.)

If you want a wardrobe, you have to find the right parts and assemble them.
(Nếu muốn có một chiếc tủ quần áo, bạn phải tìm đúng bộ phận và lắp ráp chúng.)

It’s like an appli-cation framework.
(Nó giống như một framework ứng dụng.)

The application framework offers you various pieces of software you need to build your app.
(Khung ứng dụng cung cấp cho bạn nhiều phần mềm khác nhau mà bạn cần để xây dựng ứng dụng của mình.)

You need to know what features to choose and how to assemble them to achieve the right result (figure 1.1).
(Bạn cần biết nên chọn những tính năng nào và cách lắp ráp chúng để đạt được kết quả phù hợp (hình 1.1).)

**Figure 1.1 David ordered a wardrobe from the UAssemble store. But the store (framework) doesn’t deliver to David (the programmer) just the components (software capabilities) he needs to build his new wardrobe (the app). The store ships him all the possible parts he might need to build the wardrobe. It’s David’s (the programmer’s) choice on which components (software capabilities) are right and how to assemble them to get the right result (the application).**
(Hình 1.1 David đặt mua một chiếc tủ quần áo từ cửa hàng Uassemble. Nhưng cửa hàng (khuôn khổ) không cung cấp cho David (lập trình viên) chỉ các thành phần (khả năng phần mềm) mà anh ấy cần để xây dựng tủ quần áo mới của mình (ứng dụng). Cửa hàng sẽ gửi cho anh ấy tất cả những bộ phận có thể có mà anh ấy có thể cần để đóng tủ quần áo. Đó là sự lựa chọn của David (lập trình viên) về thành phần nào (khả năng của phần mềm) là phù hợp và cách lắp ráp chúng để có được kết quả phù hợp (ứng dụng).)

The idea of a framework isn’t new.
(Ý tưởng về một framework không phải là mới.)

Throughout the history of software development, programmers observed they could reuse parts of code they’d written in multiple appli-cations.
(Trong suốt lịch sử phát triển phần mềm, các lập trình viên nhận thấy rằng họ có thể sử dụng lại các phần mã mà họ đã viết trong nhiều ứng dụng.)

Initially, when not so many applications were implemented, each application was unique and developed from scratch using a specific programming language.
(Ban đầu, khi không có nhiều ứng dụng được triển khai, mỗi ứng dụng là duy nhất và được phát triển từ đầu bằng một ngôn ngữ lập trình cụ thể.)

When the software development domain extended, and more and more applications started to be published on the market, it became easier to observe that many of these apps had similar requirements.
(Khi miền phát triển phần mềm được mở rộng và ngày càng có nhiều ứng dụng bắt đầu được xuất bản trên thị trường, việc nhận thấy nhiều ứng dụng trong số này có các yêu cầu tương tự trở nên dễ dàng hơn.)

Let’s name a few of them:
(Hãy kể tên một vài trong số họ:)

Logging error, warning, and info messages happen in every app.
(Lỗi ghi nhật ký, cảnh báo và thông báo xảy ra trong mọi ứng dụng.)

Most applications use transactions to process data changes.
(Hầu hết các ứng dụng sử dụng giao dịch để xử lý các thay đổi dữ liệu.)

Transactions repre-sent an important mechanism that takes care of data consistency.
(Các giao dịch đại diện cho một cơ chế quan trọng đảm bảo tính nhất quán của dữ liệu.)

We’ll discuss this subject in detail in chapter 13.
(Chúng ta sẽ thảo luận chi tiết về chủ đề này trong chương 13.)

Most applications use protection mechanisms against the same common vulnerabilities.
(Hầu hết các ứng dụng đều sử dụng cơ chế bảo vệ chống lại các lỗ hổng phổ biến giống nhau.)

Most applications use similar ways to communicate with each other.
(Hầu hết các ứng dụng đều sử dụng những cách tương tự để giao tiếp với nhau.)

Most applications use similar mechanisms to improve their performance, like caching or data compression.
(Hầu hết các ứng dụng đều sử dụng các cơ chế tương tự để cải thiện hiệu suất của chúng, như bộ nhớ đệm hoặc nén dữ liệu.)

And the list continues.
(Và danh sách vẫn tiếp tục.)

It turns out that the business logic code implemented in an app is significantly smaller than the wheels and belts that make the engine of the application (also often referred to as “the plumbing”).
(Hóa ra mã logic nghiệp vụ được triển khai trong một ứng dụng nhỏ hơn đáng kể so với các bánh xe và dây đai tạo nên động cơ của ứng dụng (còn thường được gọi là “hệ thống ống nước”).)

When I say “business logic code,” I refer to the code that implements the business requirements of the application.
(Khi tôi nói “mã logic nghiệp vụ”, tôi đề cập đến mã thực hiện các yêu cầu nghiệp vụ của ứng dụng.)

This code is what implements the user’s expectations in an application.
(Mã này là thứ thực hiện những mong đợi của người dùng trong một ứng dụng.)

For example, “clicking on a specific link will generate an invoice” is something users expect to happen.
(Ví dụ: “nhấp vào một liên kết cụ thể sẽ tạo ra một hóa đơn” là điều mà người dùng mong đợi sẽ xảy ra.)

Some code of the application you develop implements this functionality, and this part of code is what developers call the business logic code.
(Một số mã của ứng dụng bạn phát triển triển khai chức năng này và phần mã này được các nhà phát triển gọi là mã logic nghiệp vụ.)

However, any app takes care of several more aspects: security, logging, data con-sistency, and so on (figure 1.2).
(Tuy nhiên, bất kỳ ứng dụng nào cũng quan tâm đến một số khía cạnh khác: bảo mật, ghi nhật ký, tính nhất quán của dữ liệu, v.v. (hình 1.2).)

Business logic code
(Mã logic nghiệp vụ)

Transactions
(Giao dịch)

Caching
(Bộ nhớ đệm)

Security
(Bảo vệ)

Logging
(Ghi nhật ký)

Data transfer Data persistence
(Truyền dữ liệu Bảo tồn dữ liệu)

**Figure 1.2 The user’s perspective is like an iceberg. The users mainly observe the results of the business logic code, but this is only a small part of what builds the app’s complete functionality. Like an iceberg has most of it underwater, in an enterprise app we don’t see most of the code because it’s provided by dependencies.**
(Hình 1.2 Góc nhìn của người dùng giống như một tảng băng trôi. Người dùng chủ yếu quan sát kết quả của mã logic nghiệp vụ, nhưng đây chỉ là một phần nhỏ trong quá trình xây dựng nên chức năng hoàn chỉnh của ứng dụng. Giống như một tảng băng trôi có phần lớn nằm dưới nước, trong một ứng dụng doanh nghiệp, chúng ta không thấy hầu hết mã vì nó được cung cấp bởi các phần phụ thuộc.)

Moreover, the business logic code is what makes an application different from another from the functionality point of view.
(Hơn nữa, mã logic nghiệp vụ là thứ làm cho ứng dụng này khác với ứng dụng khác xét theo quan điểm chức năng.)

If you take two different apps, say a ride-sharing system and a social networking app, they have different use cases.
(Nếu bạn sử dụng hai ứng dụng khác nhau, chẳng hạn như hệ thống chia sẻ chuyến đi và ứng dụng mạng xã hội, chúng sẽ có các trường hợp sử dụng khác nhau.)

NOTE A use case represents the reason a person uses the app.
(LƯU Ý Trường hợp sử dụng thể hiện lý do một người sử dụng ứng dụng.)

For example, in a ridesharing app, a use case is “requesting a car.” For an app managing food delivery, a use case is “ordering a pizza.”
(Ví dụ: trong ứng dụng chia sẻ xe, trường hợp sử dụng là “yêu cầu một chiếc ô tô”. Đối với một ứng dụng quản lý dịch vụ giao đồ ăn, trường hợp sử dụng là “đặt bánh pizza”.)

You take different actions, but they both need data storing, data transfer, logging, security configurations, probably caching, and so on.
(Bạn thực hiện các hành động khác nhau nhưng cả hai đều cần lưu trữ dữ liệu, truyền dữ liệu, ghi nhật ký, cấu hình bảo mật, có thể là bộ nhớ đệm, v.v.)

Various applications can reuse these nonbusiness implementations.
(Các ứng dụng khác nhau có thể sử dụng lại các triển khai phi kinh doanh này.)

Is it then efficient to rewrite the same functionalities every time?
(Việc viết lại các chức năng giống nhau mỗi lần có hiệu quả không?)

Of course not:
(Tất nhiên là không:)

You spare a lot of time and money by reusing something rather than developing it yourself.
(Bạn tiết kiệm rất nhiều thời gian và tiền bạc bằng cách tái sử dụng thứ gì đó thay vì tự mình phát triển nó.)

An existing implementation that many apps already use has fewer chances to introduce bugs, as others have tested it.
(Cách triển khai hiện có mà nhiều ứng dụng đã sử dụng sẽ có ít cơ hội gây ra lỗi hơn vì những ứng dụng khác đã thử nghiệm nó.)

You benefit from the advice of a community because you now have a lot of developers understanding the same functionality.
(Bạn được hưởng lợi từ lời khuyên của cộng đồng vì hiện tại bạn có rất nhiều nhà phát triển hiểu được chức năng tương tự.)

If you had implemented your own code, only a few people would know it.
(Nếu bạn đã triển khai mã của riêng mình thì sẽ chỉ có một số người biết nó.)

A story of transition
(Câu chuyện chuyển tiếp)

One of the first applications I worked on was a huge system developed in Java.
(Một trong những ứng dụng đầu tiên tôi làm việc là một hệ thống khổng lồ được phát triển bằng Java.)

This system was composed of multiple applications designed around an old-fashioned architecture server, all of them written from scratch using Java SE.
(Hệ thống này bao gồm nhiều ứng dụng được thiết kế xung quanh một máy chủ có kiến ​​trúc kiểu cũ, tất cả chúng đều được viết từ đầu bằng Java SE.)

The development of this application started with the language about 25 years ago.
(Sự phát triển của ứng dụng này bắt đầu với ngôn ngữ này khoảng 25 năm trước.)

This was the main reason for its shape.
(Đây là lý do chính cho hình dạng của nó.)

And almost no one could have imagined how big it would become.
(Và hầu như không ai có thể tưởng tượng được nó sẽ lớn đến mức nào.)

At that time, more advanced concepts of system architectures didn’t exist, and things in general worked differently from the individual systems due to the slow internet connection.
(Vào thời điểm đó, các khái niệm nâng cao hơn về kiến ​​trúc hệ thống chưa tồn tại và mọi thứ nói chung hoạt động khác với các hệ thống riêng lẻ do kết nối Internet chậm.)

But time passed, and years later, the app was more like a big ball of mud.
(Nhưng thời gian trôi qua, nhiều năm sau, ứng dụng này giống như một quả bóng bùn lớn.)

For valid reasons I won’t cover here, the team decided they had to go to a modern architecture.
(Vì những lý do chính đáng mà tôi sẽ không đề cập ở đây, nhóm đã quyết định họ phải chuyển sang một kiến ​​trúc hiện đại.)

This change implied first cleaning up the code, and one of the main steps was using a framework.
(Thay đổi này ngụ ý trước tiên là phải làm sạch mã và một trong những bước chính là sử dụng một framework.)

We decided to go with Spring.
(Chúng tôi quyết định đi cùng với Spring.)

At that time, we had as an alternative Java EE (now named Jakarta EE), but most members of the team considered it’s bet-ter to go with Spring, which offered a lighter alternative that was easier to implement and that we also considered easier to maintain.
(Vào thời điểm đó, chúng tôi đã có một giải pháp thay thế Java EE (hiện có tên là Jakarta EE), nhưng hầu hết các thành viên trong nhóm cho rằng tốt hơn nên sử dụng Spring, nó cung cấp một giải pháp thay thế nhẹ hơn, dễ triển khai hơn và chúng tôi cũng cho rằng dễ bảo trì hơn.)

The transition wasn’t an easy one.
(Quá trình chuyển đổi không phải là một điều dễ dàng.)

Together with a few colleagues, experts in their domain and knowledgeable about the application itself, we invested a lot of effort into this transformation.
(Cùng với một số đồng nghiệp, chuyên gia trong lĩnh vực của họ và hiểu biết về bản thân ứng dụng, chúng tôi đã đầu tư rất nhiều công sức vào quá trình chuyển đổi này.)

The result was amazing!
(Kết quả thật tuyệt vời!)

We removed over 40% of the lines of code.
(Chúng tôi đã loại bỏ hơn 40% dòng mã.)

This transition was the first moment I understood how significant the impact of using a framework could be.
(Quá trình chuyển đổi này là khoảnh khắc đầu tiên tôi hiểu tác động của việc sử dụng một khuôn khổ có thể quan trọng như thế nào.)

NOTE Choosing and using a framework is linked to the design and architec-ture of an application.
(LƯU Ý Việc lựa chọn và sử dụng framework công tác được liên kết với thiết kế và kiến ​​trúc của một ứng dụng.)

You’ll find it useful to learn more about these subjects along with learning the Spring framework.
(Bạn sẽ thấy hữu ích khi tìm hiểu thêm về các chủ đề này cùng với việc học Spring framework.)

In appendix A, you’ll find a discus-sion about software architectures with excellent resources if you’d like to go into details.
(Trong phụ lục A, bạn sẽ tìm thấy phần thảo luận về kiến ​​trúc phần mềm với các tài nguyên tuyệt vời nếu bạn muốn đi sâu vào chi tiết.)

## The Spring Ecosystem

In this section, we will discuss Spring and related projects like Spring Boot or Spring Data.
(Trong phần này chúng ta sẽ thảo luận về Spring và các dự án liên quan như Spring Boot hay Spring Data.)

You’ll learn all about these in this book, and the links among them.
(Bạn sẽ tìm hiểu tất cả về những điều này trong cuốn sách này và các mối liên hệ giữa chúng.)

In real-world scenarios, it’s common to use different frameworks together, where each framework is designed to help you implement a specific part of the app faster.
(Trong các tình huống thực tế, việc sử dụng các framework khác nhau cùng nhau là điều phổ biến, trong đó mỗi framework được thiết kế để giúp bạn triển khai một phần cụ thể của ứng dụng nhanh hơn.)

We refer to Spring as a framework, but it is much more complex.
(Chúng tôi coi Spring như một framework, nhưng nó phức tạp hơn nhiều.)

Spring is an eco-system of frameworks.
(Mùa xuân là một hệ sinh thái của các khuôn khổ.)

Usually, when developers refer to the Spring framework, they refer to a part of the software capabilities that include the following:
(Thông thường, khi các nhà phát triển đề cập đến Spring framework, họ đề cập đến một phần khả năng của phần mềm bao gồm:)

1 Spring Core —One of the fundamental parts of Spring that includes foundational capabilities.
(1 Spring Core —Một trong những phần cơ bản của Spring bao gồm các khả năng nền tảng.)

One of these features is the Spring context.
(Một trong những tính năng này là bối cảnh mùa xuân.)

As you’ll learn in detail in chapter 2, the Spring context is a fundamental capability of the Spring framework that enables Spring to manage instances of your app.
(Như bạn sẽ tìm hiểu chi tiết trong chương 2, ngữ cảnh Spring là một khả năng cơ bản của Spring framework cho phép Spring quản lý các phiên bản ứng dụng của bạn.)

Also, as part of Spring Core, you find the Spring aspects functionality.
(Ngoài ra, là một phần của Spring Core, bạn sẽ tìm thấy chức năng của các khía cạnh Spring.)

Aspects help Spring inter-cept and manipulate methods you define in your app.
(Các khía cạnh giúp Spring chặn và thao tác các phương thức bạn xác định trong ứng dụng của mình.)

We discuss more details of the aspects in chapter 6.
(Chúng ta sẽ thảo luận chi tiết hơn về các khía cạnh trong chương 6.)

The Spring Expression Language (SpEL) is another capability you’ll find as part of Spring Core, which enables you to describe con-figurations for Spring using a specific language.
(Ngôn ngữ biểu thức mùa xuân (SpEL) là một khả năng khác mà bạn sẽ tìm thấy như một phần của Spring Core, cho phép bạn mô tả các cấu hình cho Spring bằng một ngôn ngữ cụ thể.)

All of these are new notions, and I don’t expect you to know them yet.
(Tất cả những điều này đều là những khái niệm mới và tôi không mong bạn biết chúng.)

But soon you’ll understand that Spring Core holds the mechanisms Spring uses to integrate into your app.
(Nhưng bạn sẽ sớm hiểu rằng Spring Core nắm giữ các cơ chế mà Spring sử dụng để tích hợp vào ứng dụng của bạn.)

2 Spring model-view-controller (MVC) —The part of the Spring framework that enables you to develop web applications that serve HTTP requests.
(2 Spring model-view-controller (MVC) —Một phần của Spring framework cho phép bạn phát triển các ứng dụng web phục vụ các yêu cầu HTTP.)

We’ll use Spring MVC starting in chapter 7.
(Chúng ta sẽ sử dụng Spring MVC bắt đầu từ chương 7.)

3 Spring Data Access —Also one of the fundamental parts of Spring.
(3 Truy cập dữ liệu Spring —Cũng là một trong những phần cơ bản của Spring.)

It provides basic tools you can use to connect to SQL databases to implement the per-sistence layer of your app.
(Nó cung cấp các công cụ cơ bản mà bạn có thể sử dụng để kết nối với cơ sở dữ liệu SQL nhằm triển khai lớp duy trì lâu dài của ứng dụng.)

We’ll use Spring Data Access starting in chapter 13.
(Chúng ta sẽ sử dụng Truy cập dữ liệu Spring bắt đầu từ chương 13.)

4 Spring testing—The part holding the tools you need to write tests for your Spring application.
(4 Spring testing—Phần chứa các công cụ bạn cần để viết test cho ứng dụng Spring của mình.)

We’ll discuss this subject in chapter 15.
(Chúng ta sẽ thảo luận về chủ đề này trong chương 15.)

You can initially imagine the Spring framework as a solar system, where Spring Core represents the star in the middle, which holds all the framework together (figure 1.3).
(Ban đầu bạn có thể hình dung Spring framework như một hệ mặt trời, trong đó Spring Core đại diện cho ngôi sao ở giữa, giữ tất cả các framework lại với nhau (hình 1.3).)

Spring MVC
(Mùa xuân MVC)

Spring testing
(Thử nghiệm mùa xuân)

Spring Core
(Lõi lò xo)

Spring Data Access
(Truy cập dữ liệu mùa xuân)

**Figure 1.3 You can imagine the Spring framework as a solar system with the Spring Core in the center. The software capabilities are planets around Spring Core kept close to it by its gravitational field.**
(Hình 1.3 Bạn có thể tưởng tượng Spring framework như một hệ mặt trời với Spring Core ở trung tâm. Khả năng của phần mềm là các hành tinh xung quanh Spring Core được giữ gần nó bởi trường hấp dẫn của nó.)

The Spring framework (shortly, Spring) is an application framework that is part of the Java ecosystem.(Spring framework (gọi tắt là Spring) là một framework ứng dụng thuộc hệ sinh thái Java.)
(Spring framework (gọi tắt là Spring) là một framework ứng dụng nằm trong hệ sinh thái Java.(Spring framework (gọi tắt là Spring) là một framework ứng dụng thuộc hệ sinh thái Java.))

An application framework is a set of common software functionalities that provides a foundation structure for developing an application.(Một framework ứng dụng là một tập hợp các chức năng phần mềm chung cung cấp cấu trúc nền tảng để phát triển một ứng dụng.)An application framework eases the effort of writing an application by taking out the effort of writing all the program code from scratch.(Một framework ứng dụng giúp giảm bớt nỗ lực viết ứng dụng bằng cách loại bỏ việc phải viết toàn bộ mã chương trình từ đầu.)
(Khung ứng dụng là một tập hợp các chức năng phần mềm phổ biến cung cấp cấu trúc nền tảng để phát triển một ứng dụng. (Một framework ứng dụng là một tập hợp các chức năng phần mềm chung cung cấp cấu trúc nền để phát triển một ứng dụng.) Khung ứng dụng giúp giảm bớt nỗ lực viết một ứng dụng bằng cách loại bỏ nỗ lực viết tất cả mã chương trình từ đầu. (Một framework ứng dụng giúp giảm bớt lực viết ứng dụng bằng cách loại bỏ việc bỏ phải viết toàn bộ mã chương trình.))

We use Spring in the development of many kinds of applications nowadays, from large backend solutions to automation testing apps.(Ngày nay, chúng ta sử dụng Spring để phát triển nhiều loại ứng dụng, từ các giải pháp backend lớn đến các ứng dụng kiểm thử tự động.)According to many survey reports on Java technologies, Spring is the most used Java framework today.(Theo nhiều báo cáo khảo sát về công nghệ Java, hiện nay Spring là framework Java được sử dụng nhiều nhất.)
(Hiện nay, chúng tôi sử dụng Spring để phát triển nhiều loại ứng dụng, từ các giải pháp phụ trợ lớn đến các ứng dụng thử nghiệm tự động hóa. (Ngày nay, chúng tôi sử dụng Spring để phát triển nhiều loại ứng dụng, từ các giải pháp phụ trợ đến các ứng dụng kiểm tra tự động.)Theo nhiều báo cáo khảo sát về công nghệ Java, Spring là framework Java được sử dụng nhiều nhất hiện nay. (Theo nhiều báo cáo khảo sát về công nghệ Java, hiện nay Spring là framework Java được sử dụng nhiều nhất.))

Spring is popular, and developers have started to use it more often with other JVM languages than Java as well.(Spring rất phổ biến, và các lập trình viên cũng bắt đầu sử dụng nó thường xuyên hơn với các ngôn ngữ JVM khác ngoài Java.)
(Spring rất phổ biến và các nhà phát triển cũng bắt đầu sử dụng nó thường xuyên hơn với các ngôn ngữ JVM khác ngoài Java.(Spring rất phổ biến và các lập trình viên cũng bắt đầu sử dụng thường xuyên hơn so với các ngôn ngữ JVM khác ngoài Java.))

write, which defines the logic of the app.
(write, xác định logic của ứng dụng.)

Here’s where the “inversion” in IoC comes from: you don’t let the app control the execution by its own code and use dependen-cies.
(Đây là nguồn gốc của sự “đảo ngược” trong IoC: bạn không để ứng dụng kiểm soát việc thực thi bằng mã riêng của nó và sử dụng các phần phụ thuộc.)

Instead, we allow the framework (the dependency) to control the app and its code (figure 1.4).
(Thay vào đó, chúng tôi cho phép framework (phần phụ thuộc) kiểm soát ứng dụng và mã của nó (hình 1.4).)

NOTE In this context the term “controls” refers to actions like “creating an instance” or “calling a method.” A framework can create objects of the classes you define in your app.
(LƯU Ý Trong ngữ cảnh này, thuật ngữ “điều khiển” đề cập đến các hành động như “tạo một phiên bản” hoặc “gọi một phương thức”. Một framework có thể tạo các đối tượng của các lớp mà bạn xác định trong ứng dụng của mình.)

Based on the configurations that you write, Spring intercepts the method to augment it with various features.
(Dựa trên các cấu hình mà bạn viết, Spring chặn phương thức này để tăng cường nó bằng nhiều tính năng khác nhau.)

For example, Spring can intercept a specific method to log any error that might appear during the method’s execution.
(Ví dụ: Spring có thể chặn một phương thức cụ thể để ghi lại bất kỳ lỗi nào có thể xuất hiện trong quá trình thực thi phương thức đó.)

Without IoC
(Không có IoC)

The application executes and controls (uses) the dependencies it needs.
(Ứng dụng thực thi và kiểm soát (sử dụng) các phần phụ thuộc mà nó cần.)

In the last few years, we observed an impressive growth of developers using Spring with Kotlin (another appreciated language from the JVM family).(Trong những năm gần đây, số lượng lập trình viên sử dụng Spring với Kotlin, một ngôn ngữ được đánh giá cao trong hệ JVM, đã tăng trưởng ấn tượng.)In this book, we'll focus on the foundations of Spring, and I'll teach you essential skills for using Spring in real-world examples.(Trong cuốn sách này, chúng ta sẽ tập trung vào nền tảng của Spring, và tôi sẽ hướng dẫn bạn những kỹ năng cốt lõi để sử dụng Spring trong các ví dụ thực tế.)To make the subject more comfortable for you and allow you to focus on Spring, we'll use only Java examples.(Để giúp nội dung dễ tiếp cận hơn và để bạn tập trung vào Spring, chúng ta sẽ chỉ sử dụng các ví dụ bằng Java.)Throughout the book, we'll discuss and apply, with examples, essential skills like connecting to a database, establishing communication between applications, and securing and testing an app.(Xuyên suốt cuốn sách, chúng ta sẽ thảo luận và áp dụng qua ví dụ các kỹ năng quan trọng như kết nối cơ sở dữ liệu, thiết lập giao tiếp giữa các ứng dụng, cũng như bảo mật và kiểm thử ứng dụng.)
(Trong vài năm gần đây, chúng tôi đã quan sát thấy sự tăng trưởng ấn tượng của số lượng nhà phát triển sử dụng Spring với Kotlin (một ngôn ngữ được đánh giá cao khác từ gia đình JVM).(Trong những năm gần đây, số lượng lập trình viên sử dụng Spring với Kotlin, một ngôn ngữ được đánh giá cao trong hệ thống JVM, đã tăng ấn tượng.)Trong cuốn sách này, chúng tôi sẽ tập trung vào nền tảng của Spring và tôi sẽ dạy bạn những kỹ năng cần thiết để sử dụng Spring trong các ví dụ thực tế.(Trong cuốn sách này, chúng tôi sẽ tập trung vào nền tảng của Spring, và tôi sẽ hướng dẫn bạn những kỹ năng cốt lõi để sử dụng Spring trong các ví dụ thực tế.)Để làm cho chủ đề thoải mái hơn cho bạn và cho phép bạn tập trung vào Spring, chúng tôi sẽ chỉ sử dụng các ví dụ Java.(Để giúp nội dung dễ tiếp cận hơn và để bạn tập trung vào Spring, chúng tôi sẽ chỉ sử dụng các ví dụ bằng Java.) Xuyên suốt cuốn sách, chúng ta sẽ thảo luận và áp dụng, kèm theo các ví dụ, các kỹ năng cần thiết như kết nối với cơ sở dữ liệu, thiết lập giao tiếp giữa các ứng dụng cũng như bảo mật và thử nghiệm một ứng dụng. sách, chúng tôi sẽ thảo luận và áp dụng các ví dụ về các kỹ năng quan trọng như kết nối cơ sở dữ liệu, thiết lập giao diện tiếp theo giữa các ứng dụng, cũng như bảo mật và kiểm tra ứng dụng.))

Before diving into more technical details in the next chapters, let's talk about the Spring framework and where you'll actually use it.(Trước khi đi sâu hơn vào các chi tiết kỹ thuật ở những chương tiếp theo, hãy cùng nói về Spring framework và những nơi bạn thực sự sẽ sử dụng nó.)Why is Spring so appreciated, and when should you even use it?
(Trước khi đi sâu vào chi tiết kỹ thuật hơn trong các chương tiếp theo, hãy nói về Spring framework và nơi bạn sẽ thực sự sử dụng nó.(Trước khi đi sâu hơn vào các chi tiết kỹ thuật ở những chương trình tiếp theo, hãy cùng nói về Spring framework và những nơi bạn thực sự sẽ sử dụng nó.)Tại sao Spring được đánh giá cao như vậy và khi nào bạn nên sử dụng nó?)

ControlsDependencyDependencyDependencyControlsDependencyDependencyDependencyApplication
(Điều khiểnPhụ thuộcPhụ thuộcPhụ thuộcĐiều khiểnPhụ thuộcPhụ thuộcPhụ thuộcỨng dụng)

ControlsApplicationControlsApplicationWith IoC
(Điều khiểnỨng dụngĐiều khiểnỨng dụngVới IoC)

The application executes being controlled by the framework (dependency).
(Ứng dụng thực thi được kiểm soát bởi framework (phụ thuộc).)

Framework (dependency)
(Khung (phụ thuộc))

**Figure 1.4 Inversion of control. Instead of executing its own code, which makes use of several other dependencies, in case of an IoC scenario, the app execution is controlled by the dependency. The Spring framework controls an app during its execution. Therefore, it implements an IoC scenario of execution.**
(Hình 1.4 Đảo ngược điều khiển. Thay vì thực thi mã của chính nó, sử dụng một số phần phụ thuộc khác, trong trường hợp kịch bản IoC, việc thực thi ứng dụng được kiểm soát bởi phần phụ thuộc. Khung công tác Spring kiểm soát một ứng dụng trong quá trình thực thi. Do đó, nó thực hiện một kịch bản thực thi IoC.)

You will start learning Spring with Spring Core by discussing the Spring IoC function-ality in chapters 2 through 5.
(Bạn sẽ bắt đầu học Spring với Spring Core bằng cách thảo luận về chức năng Spring IoC trong chương 2 đến chương 5.)

The IoC container glues Spring components and components of your application to the framework together.
(Bộ chứa IoC gắn các thành phần Spring và các thành phần của ứng dụng của bạn vào framework với nhau.)

Using the IoC container, to which you often refer as the Spring context, you make certain objects known to Spring, which enables the framework to use them in the way you configured.
(Bằng cách sử dụng bộ chứa IoC, mà bạn thường gọi là bối cảnh Spring, bạn làm cho một số đối tượng nhất định được biết đến với Spring, điều này cho phép framework sử dụng chúng theo cách bạn đã định cấu hình.)

In chapter 6, we’ll continue our discussion with Spring aspect-oriented programming (AOP).
(Trong chương 6, chúng ta sẽ tiếp tục thảo luận về lập trình hướng theo khía cạnh Spring (AOP).)

Spring can control instances added to its IoC container, and one of the things it can do is intercept methods that represent the behavior of these instances.
(Spring có thể kiểm soát các phiên bản được thêm vào bộ chứa IoC của nó và một trong những điều nó có thể làm là chặn các phương thức thể hiện hành vi của các phiên bản này.)

This capability is called aspecting the method.
(Khả năng này được gọi là khía cạnh phương pháp.)

Spring AOP is one of the most common ways the framework interacts with what your app does.
(Spring AOP là một trong những cách phổ biến nhất mà framework tương tác với ứng dụng của bạn.)

This trait makes Spring AOP part of the essentials as well.
(Đặc điểm này làm cho Spring AOP trở thành một phần thiết yếu.)

Part of the Spring Core, we also find resource management,
(Một phần của Spring Core, chúng tôi cũng tìm thấy tính năng quản lý tài nguyên,)

internationalization (i18n), type conversion, and SpEL.
(quốc tế hóa (i18n), chuyển đổi loại và SpEL.)

We’ll encounter aspects of these features in examples throughout the book.
(Chúng ta sẽ gặp các khía cạnh của những đặc điểm này trong các ví dụ xuyên suốt cuốn sách.)

Using Spring Data Access feature to implement the app’s persistence
(Sử dụng tính năng Spring Data Access để triển khai tính bền vững của ứng dụng)

For most applications, it’s critical to persist part of the data they process.
(Đối với hầu hết các ứng dụng, điều quan trọng là phải duy trì một phần dữ liệu mà chúng xử lý.)

Working with databases is a fundamental subject, and in Spring, it’s the Data Access module that you’ll use to take care of data persistence in many cases.
(Làm việc với cơ sở dữ liệu là một chủ đề cơ bản và trong Spring, đó là mô-đun Truy cập dữ liệu mà bạn sẽ sử dụng để đảm bảo tính bền vững của dữ liệu trong nhiều trường hợp.)

The Spring Data Access includes using JDBC, integrating with object-relational mapping (ORM) frameworks like Hibernate (don’t worry if you don’t yet know what an ORM framework is or haven’t heard about Hibernate; we’ll discuss these aspects later in the book), and managing transactions.
(Truy cập dữ liệu Spring bao gồm sử dụng JDBC, tích hợp với các framework ánh xạ quan hệ đối tượng (ORM) như Hibernate (đừng lo lắng nếu bạn chưa biết framework ORM là gì hoặc chưa nghe nói về Hibernate; chúng ta sẽ thảo luận về các khía cạnh này sau trong cuốn sách) và quản lý các giao dịch.)

In chapters 12 through 14, we’ll cover everything needed to get you started with Spring Data Access.
(Trong các chương 12 đến 14, chúng tôi sẽ đề cập đến mọi thứ cần thiết để giúp bạn bắt đầu với Spring Data Access.)

The Spring MVC capabilities for developing web apps
(Các khả năng của Spring MVC để phát triển ứng dụng web)

The most common applications developed with Spring are web apps, and within the Spring ecosystem, you’ll find a large set of tools that enables you to write web applications and web services in different fashions.
(Các ứng dụng phổ biến nhất được phát triển với Spring là các ứng dụng web và trong hệ sinh thái Spring, bạn sẽ tìm thấy một bộ công cụ lớn cho phép bạn viết các ứng dụng web và dịch vụ web theo nhiều kiểu khác nhau.)

You can use the Spring MVC to develop apps using a standard servlet fashion, which is common in a vast number of applications today.
(Bạn có thể sử dụng Spring MVC để phát triển ứng dụng bằng cách sử dụng kiểu servlet tiêu chuẩn, kiểu này phổ biến trong rất nhiều ứng dụng hiện nay.)

In chapter 7, we’ll go into more detail on using the Spring MVC.
(Trong chương 7, chúng ta sẽ đi vào chi tiết hơn về cách sử dụng Spring MVC.)

The Spring testing feature
(Tính năng kiểm tra mùa xuân)

The Spring testing module offers us a large set of tools that we’ll use to write unit and integration tests.
(Mô-đun kiểm thử Spring cung cấp cho chúng ta một bộ công cụ lớn mà chúng ta sẽ sử dụng để viết các bài kiểm thử đơn vị và tích hợp.)

There have been many pages written about the testing topic, but we’ll discuss everything that is essential to get you started with Spring testing in chapter 15.
(Đã có nhiều trang viết về chủ đề kiểm thử, nhưng chúng ta sẽ thảo luận mọi thứ cần thiết để giúp bạn bắt đầu kiểm thử Spring ở chương 15.)

I’ll also refer to some valuable resources you need to read to get all the details of this topic.
(Tôi cũng sẽ đề cập đến một số tài nguyên có giá trị mà bạn cần đọc để biết tất cả thông tin chi tiết về chủ đề này.)

My rule of thumb is that you’re not a mature developer if you don’t understand testing, so this topic is one you should care about.
(Nguyên tắc nhỏ của tôi là bạn không phải là nhà phát triển trưởng thành nếu bạn không hiểu về kiểm thử, vì vậy chủ đề này là chủ đề bạn nên quan tâm.)

Projects from the Spring ecosystem
(Các dự án từ hệ sinh thái Spring)

The Spring ecosystem is so much more than just the capabilities discussed earlier in this section.
(Hệ sinh thái Spring không chỉ có những khả năng được thảo luận trước đó trong phần này.)

It includes a big collection of other frameworks that integrate well and form a larger universe.
(Nó bao gồm một bộ sưu tập lớn các framework khác tích hợp tốt và tạo thành một vũ trụ lớn hơn.)

Here we have projects like Spring Data, Spring Security, Spring Cloud, Spring Batch, Spring Boot, and so on.
(Ở đây chúng tôi có các dự án như Spring Data, Spring Security, Spring Cloud, Spring Batch, Spring Boot, v.v.)

When you develop an app, you can use more of these projects together.
(Khi bạn phát triển một ứng dụng, bạn có thể sử dụng nhiều dự án này cùng nhau.)

For example, you can build an app using all of Spring Boot, Spring Security, and Spring Data.
(Ví dụ: bạn có thể xây dựng một ứng dụng bằng cách sử dụng tất cả Spring Boot, Spring Security và Spring Data.)

In the next few chapters, we’ll work on smaller projects that make use of various projects of the Spring ecosystem.
(Trong một số chương tiếp theo, chúng ta sẽ làm việc trên các dự án nhỏ hơn sử dụng nhiều dự án khác nhau của hệ sinh thái Spring.)

When I say project, I refer to a part of the Spring ecosystem that is independently developed.
(Khi nói đến dự án, tôi muốn nói đến một phần của hệ sinh thái Spring được phát triển độc lập.)

Each of these projects has a separate team that works on extending its capabilities.
(Mỗi dự án này có một nhóm riêng biệt làm việc để mở rộng khả năng của mình.)

Also, each project is separately described and has its own reference on the Spring official web-site: https://spring.io/projects.
(Ngoài ra, mỗi dự án được mô tả riêng và có tài liệu tham khảo riêng trên trang web chính thức của Spring: https://spring.io/projects.)

Out of this vast universe created by Spring, we’ll also refer to Spring Data and Spring Boot.
(Ngoài vũ trụ rộng lớn do Spring tạo ra này, chúng ta cũng sẽ đề cập đến Spring Data và Spring Boot.)

These projects are often encountered in apps, so it’s important to get to know them from the beginning.
(Những dự án này thường gặp trong ứng dụng, vì vậy điều quan trọng là bạn phải tìm hiểu chúng ngay từ đầu.)

Extending the persistence capabilities with Spring Data
(Mở rộng khả năng kiên trì với Spring Data)

The Spring Data project implements a part of the Spring ecosystem that enables you to easily connect to databases and use the persistence layer with a minimum number of lines of code written.
(Dự án Spring Data triển khai một phần của hệ sinh thái Spring cho phép bạn dễ dàng kết nối với cơ sở dữ liệu và sử dụng lớp lưu giữ lâu dài với số dòng mã được viết tối thiểu.)

The project refers to both SQL and NoSQL technologies and creates a high-level layer, which simplifies the way you work with data persistence.
(Dự án đề cập đến cả công nghệ SQL và NoSQL, đồng thời tạo ra một lớp cấp cao, giúp đơn giản hóa cách bạn làm việc với tính lưu giữ dữ liệu.)

NOTE We have Spring Data Access, which is a module of Spring Core, and we also have an independent project in the Spring ecosystem named Spring Data.
(LƯU Ý Chúng tôi có Spring Data Access, là một mô-đun của Spring Core và chúng tôi cũng có một dự án độc lập trong hệ sinh thái Spring có tên Spring Data.)

Spring Data Access contains fundamental data access implementations like the transaction mechanism and JDBC tools.
(Truy cập dữ liệu mùa xuân chứa các triển khai truy cập dữ liệu cơ bản như cơ chế giao dịch và các công cụ JDBC.)

Spring Data enhances access to databases and offers a broader set of tools, which makes development more accessible and enables your app to connect to different kinds of data sources.
(Spring Data tăng cường quyền truy cập vào cơ sở dữ liệu và cung cấp bộ công cụ rộng hơn, giúp việc phát triển dễ tiếp cận hơn và cho phép ứng dụng của bạn kết nối với các loại nguồn dữ liệu khác nhau.)

We’ll discuss this subject in chapter 14.
(Chúng ta sẽ thảo luận về chủ đề này trong chương 14.)

Spring Boot
(Khởi động mùa xuân)

Spring Boot is a project part of the Spring ecosystem that introduces the concept of “convention over configuration.” The main idea of this concept is that instead of set-ting up all the configurations of a framework yourself, Spring Boot offers you a default configuration that you can customize as needed.
(Spring Boot là một phần dự án của hệ sinh thái Spring giới thiệu khái niệm “quy ước về cấu hình”. Ý tưởng chính của khái niệm này là thay vì tự mình thiết lập tất cả các cấu hình của một framework, Spring Boot cung cấp cho bạn một cấu hình mặc định mà bạn có thể tùy chỉnh khi cần.)

The result, in general, is that you write less code because you follow known conventions and your app differs from others in few or small ways.
(Nói chung, kết quả là bạn viết ít mã hơn vì bạn tuân theo các quy ước đã biết và ứng dụng của bạn khác với các ứng dụng khác ở một vài điểm hoặc một số điểm nhỏ.)

So instead of writing all the configurations for each and every app, it’s more efficient to start with a default configuration and only change what’s different from the convention.
(Vì vậy, thay vì viết tất cả cấu hình cho từng ứng dụng, sẽ hiệu quả hơn nếu bắt đầu với cấu hình mặc định và chỉ thay đổi những gì khác với quy ước.)

We’ll discuss more about Spring Boot starting in chapter 7.
(Chúng ta sẽ thảo luận thêm về Spring Boot bắt đầu từ chương 7.)

The Spring ecosystem is vast and contains many projects.
(Hệ sinh thái Spring rất rộng lớn và chứa nhiều dự án.)

Some of them you encounter more often than others, and some you may not use at all if you’re building an application without a particular need.
(Một số trong số chúng bạn gặp thường xuyên hơn những thứ khác và một số bạn có thể không sử dụng chút nào nếu bạn đang xây dựng một ứng dụng mà không có nhu cầu cụ thể.)

In this book, we refer only to the projects that are essential for you to get started: Spring Core, Spring Data, and Spring Boot.
(Trong cuốn sách này, chúng tôi chỉ đề cập đến các dự án cần thiết để bạn bắt đầu: Spring Core, Spring Data và Spring Boot.)

You can find a full list of projects that are part of the Spring ecosystem on the official
(Bạn có thể tìm thấy danh sách đầy đủ các dự án thuộc hệ sinh thái Spring trên trang chính thức)

Spring website: https://spring.io/projects/.
(Trang web mùa xuân: https://spring.io/projects/.)

Alternatives for using SpringWe can’t really discuss alternatives to Spring because someone could misunderstand them as alternatives to the entire ecosystem.
(Các lựa chọn thay thế cho việc sử dụng SpringChúng tôi thực sự không thể thảo luận về các lựa chọn thay thế cho Spring vì ai đó có thể hiểu nhầm chúng là những lựa chọn thay thế cho toàn bộ hệ sinh thái.)

But for many of the individual components and projects that create the Spring ecosystem, you can find other options like other open source or commercial frameworks or libraries.For example, let’s take the Spring IoC container.
(Nhưng đối với nhiều thành phần và dự án riêng lẻ tạo ra hệ sinh thái Spring, bạn có thể tìm thấy các tùy chọn khác như các framework hoặc thư viện nguồn mở hoặc thương mại khác. Ví dụ: hãy lấy bộ chứa Spring IoC.)

Years ago, the Java EE specification was a solution very much appreciated by the developers.
(Nhiều năm trước, đặc tả Java EE là một giải pháp được các nhà phát triển đánh giá rất cao.)

With a slightly different philosophy, Java EE (which in 2017 was open sourced and remade in Jakarta EE, https://jakarta.ee/) offered specifications like Context and Dependency Injection (CDI) or Enterprise Java Beans (EJB).
(Với triết lý hơi khác một chút, Java EE (năm 2017 là mã nguồn mở và được làm lại ở Jakarta EE, https://jakarta.ee/) đã cung cấp các thông số kỹ thuật như Context and Dependency Insert (CDI) hoặc Enterprise Java Beans (EJB).)

You could use CDI or EJB to manage a context of object instances and implement aspects (named “interceptors” in the EE terminol-ogy).
(Bạn có thể sử dụng CDI hoặc EJB để quản lý ngữ cảnh của các thể hiện đối tượng và các khía cạnh triển khai (được đặt tên là “các bộ chặn” trong thuật ngữ EE).)

Also, throughout history, Google Guice (https://github.com/google/guice) was an appreciated framework for the management of object instances in a container.Alternatives for using SpringWe can’t really discuss alternatives to Spring because someone could misunderstand them as alternatives to the entire ecosystem.
(Ngoài ra, trong suốt lịch sử, Google Guice (https://github.com/google/guice) là một framework được đánh giá cao để quản lý các phiên bản đối tượng trong vùng chứa. Các lựa chọn thay thế để sử dụng SpringChúng tôi thực sự không thể thảo luận về các lựa chọn thay thế cho Spring vì ai đó có thể hiểu nhầm chúng là các lựa chọn thay thế cho toàn bộ hệ sinh thái.)

But for many of the individual components and projects that create the Spring ecosystem, you can find other options like other open source or commercial frameworks or libraries.For example, let’s take the Spring IoC container.
(Nhưng đối với nhiều thành phần và dự án riêng lẻ tạo ra hệ sinh thái Spring, bạn có thể tìm thấy các tùy chọn khác như các framework hoặc thư viện nguồn mở hoặc thương mại khác. Ví dụ: hãy lấy bộ chứa Spring IoC.)

Years ago, the Java EE specification was a solution very much appreciated by the developers.
(Nhiều năm trước, đặc tả Java EE là một giải pháp được các nhà phát triển đánh giá rất cao.)

With a slightly different philosophy, Java EE (which in 2017 was open sourced and remade in Jakarta EE, https://jakarta.ee/) offered specifications like Context and Dependency Injection (CDI) or Enterprise Java Beans (EJB).
(Với triết lý hơi khác một chút, Java EE (năm 2017 là mã nguồn mở và được làm lại ở Jakarta EE, https://jakarta.ee/) đã cung cấp các thông số kỹ thuật như Context and Dependency Insert (CDI) hoặc Enterprise Java Beans (EJB).)

You could use CDI or EJB to manage a context of object instances and implement aspects (named “interceptors” in the EE terminol-ogy).
(Bạn có thể sử dụng CDI hoặc EJB để quản lý ngữ cảnh của các thể hiện đối tượng và các khía cạnh triển khai (được đặt tên là “các bộ chặn” trong thuật ngữ EE).)

Also, throughout history, Google Guice (https://github.com/google/guice) was an appreciated framework for the management of object instances in a container.
(Ngoài ra, trong suốt lịch sử, Google Guice (https://github.com/google/guice) là một framework được đánh giá cao để quản lý các phiên bản đối tượng trong vùng chứa.)

Alternatives for using Spring
(Các lựa chọn thay thế cho việc sử dụng Spring)

We can’t really discuss alternatives to Spring because someone could misunderstand them as alternatives to the entire ecosystem.
(Chúng ta thực sự không thể thảo luận về các lựa chọn thay thế cho Spring vì ai đó có thể hiểu nhầm chúng là những lựa chọn thay thế cho toàn bộ hệ sinh thái.)

But for many of the individual components and projects that create the Spring ecosystem, you can find other options like other open source or commercial frameworks or libraries.
(Nhưng đối với nhiều thành phần và dự án riêng lẻ tạo ra hệ sinh thái Spring, bạn có thể tìm thấy các tùy chọn khác như các thư viện hoặc framework thương mại hoặc nguồn mở khác.)

For example, let’s take the Spring IoC container.
(Ví dụ: hãy lấy bộ chứa Spring IoC.)

Years ago, the Java EE specification was a solution very much appreciated by the developers.
(Nhiều năm trước, đặc tả Java EE là một giải pháp được các nhà phát triển đánh giá rất cao.)

With a slightly different philosophy, Java EE (which in 2017 was open sourced and remade in Jakarta EE, https://jakarta.ee/) offered specifications like Context and Dependency Injection (CDI) or Enterprise Java Beans (EJB).
(Với triết lý hơi khác một chút, Java EE (năm 2017 là mã nguồn mở và được làm lại ở Jakarta EE, https://jakarta.ee/) đã cung cấp các thông số kỹ thuật như Context and Dependency Insert (CDI) hoặc Enterprise Java Beans (EJB).)

You could use CDI or EJB to manage a context of object instances and implement aspects (named “interceptors” in the EE terminol-ogy).
(Bạn có thể sử dụng CDI hoặc EJB để quản lý ngữ cảnh của các thể hiện đối tượng và các khía cạnh triển khai (được đặt tên là “các bộ chặn” trong thuật ngữ EE).)

Also, throughout history, Google Guice (https://github.com/google/guice) was an appreciated framework for the management of object instances in a container.
(Ngoài ra, trong suốt lịch sử, Google Guice (https://github.com/google/guice) là một framework được đánh giá cao để quản lý các phiên bản đối tượng trong vùng chứa.)

Alternatives for using Spring
(Các lựa chọn thay thế cho việc sử dụng Spring)

We can’t really discuss alternatives to Spring because someone could misunderstand them as alternatives to the entire ecosystem.
(Chúng ta thực sự không thể thảo luận về các lựa chọn thay thế cho Spring vì ai đó có thể hiểu nhầm chúng là những lựa chọn thay thế cho toàn bộ hệ sinh thái.)

But for many of the individual components and projects that create the Spring ecosystem, you can find other options like other open source or commercial frameworks or libraries.
(Nhưng đối với nhiều thành phần và dự án riêng lẻ tạo ra hệ sinh thái Spring, bạn có thể tìm thấy các tùy chọn khác như các thư viện hoặc framework thương mại hoặc nguồn mở khác.)

For example, let’s take the Spring IoC container.
(Ví dụ: hãy lấy bộ chứa Spring IoC.)

Years ago, the Java EE specification was a solution very much appreciated by the developers.
(Nhiều năm trước, đặc tả Java EE là một giải pháp được các nhà phát triển đánh giá rất cao.)

With a slightly different philosophy, Java EE (which in 2017 was open sourced and remade in Jakarta EE, https://jakarta.ee/) offered specifications like Context and Dependency Injection (CDI) or Enterprise Java Beans (EJB).
(Với triết lý hơi khác một chút, Java EE (năm 2017 là mã nguồn mở và được làm lại ở Jakarta EE, https://jakarta.ee/) đã cung cấp các thông số kỹ thuật như Context and Dependency Insert (CDI) hoặc Enterprise Java Beans (EJB).)

You could use CDI or EJB to manage a context of object instances and implement aspects (named “interceptors” in the EE terminol-ogy).
(Bạn có thể sử dụng CDI hoặc EJB để quản lý ngữ cảnh của các thể hiện đối tượng và các khía cạnh triển khai (được đặt tên là “các bộ chặn” trong thuật ngữ EE).)

Also, throughout history, Google Guice (https://github.com/google/guice) was an appreciated framework for the management of object instances in a container.
(Ngoài ra, trong suốt lịch sử, Google Guice (https://github.com/google/guice) là một framework được đánh giá cao để quản lý các phiên bản đối tượng trong vùng chứa.)

(continued)For some of the projects taken individually, you could find one or more alternatives.
((tiếp theo) Đối với một số dự án được thực hiện riêng lẻ, bạn có thể tìm thấy một hoặc nhiều lựa chọn thay thế.)

For example, you could choose to use Apache Shiro (https://shiro.apache.org/) instead of Spring Security.
(Ví dụ: bạn có thể chọn sử dụng Apache Shira (https://shiro.apache.org/) thay vì Spring Security.)

Or you could decide to implement your web app using the Play framework (https://www.playframework.com/) instead of Spring MVC and Spring-related technologies.A more recent project that looks promising is Red Hat Quarkus.
(Hoặc bạn có thể quyết định triển khai ứng dụng web của mình bằng cách sử dụng framework Play (https://www.playframework.com/) thay vì Spring MVC và các công nghệ liên quan đến Spring. Một dự án gần đây hơn có vẻ đầy hứa hẹn là Red Hat Quarkus.)

Quarkus is designed for cloud native implementations and becomes more and more mature with rapid steps.
(Quarkus được thiết kế để triển khai trên nền tảng đám mây và ngày càng hoàn thiện hơn với các bước nhanh chóng.)

I wouldn’t be surprised to see it as one of the lead projects in developing enter-prise apps in the Java ecosystem in the future (https://quarkus.io/).My advice for you is to always take into consideration your alternatives.
(Tôi sẽ không ngạc nhiên khi coi đây là một trong những dự án hàng đầu trong việc phát triển các ứng dụng dành cho doanh nghiệp trong hệ sinh thái Java trong tương lai (https://quarkus.io/). Lời khuyên của tôi dành cho bạn là hãy luôn cân nhắc các lựa chọn thay thế của mình.)

In software development, you need to be open-minded and never trust one solution as being “the one.” You’ll always find scenarios in which a specific technology works better than another.(continued)For some of the projects taken individually, you could find one or more alternatives.
(Trong quá trình phát triển phần mềm, bạn cần phải có tư duy cởi mở và không bao giờ tin tưởng vào một giải pháp là “duy nhất”. Bạn sẽ luôn tìm thấy các tình huống trong đó một công nghệ cụ thể hoạt động tốt hơn công nghệ khác. (tiếp theo) Đối với một số dự án được thực hiện riêng lẻ, bạn có thể tìm thấy một hoặc nhiều lựa chọn thay thế.)

For example, you could choose to use Apache Shiro (https://shiro.apache.org/) instead of Spring Security.
(Ví dụ: bạn có thể chọn sử dụng Apache Shira (https://shiro.apache.org/) thay vì Spring Security.)

Or you could decide to implement your web app using the Play framework (https://www.playframework.com/) instead of Spring MVC and Spring-related technologies.A more recent project that looks promising is Red Hat Quarkus.
(Hoặc bạn có thể quyết định triển khai ứng dụng web của mình bằng cách sử dụng framework Play (https://www.playframework.com/) thay vì Spring MVC và các công nghệ liên quan đến Spring. Một dự án gần đây hơn có vẻ đầy hứa hẹn là Red Hat Quarkus.)

Quarkus is designed for cloud native implementations and becomes more and more mature with rapid steps.
(Quarkus được thiết kế để triển khai trên nền tảng đám mây và ngày càng hoàn thiện hơn với các bước nhanh chóng.)

I wouldn’t be surprised to see it as one of the lead projects in developing enter-prise apps in the Java ecosystem in the future (https://quarkus.io/).My advice for you is to always take into consideration your alternatives.
(Tôi sẽ không ngạc nhiên khi coi đây là một trong những dự án hàng đầu trong việc phát triển các ứng dụng dành cho doanh nghiệp trong hệ sinh thái Java trong tương lai (https://quarkus.io/). Lời khuyên của tôi dành cho bạn là hãy luôn cân nhắc các lựa chọn thay thế của mình.)

In software development, you need to be open-minded and never trust one solution as being “the one.” You’ll always find scenarios in which a specific technology works better than another.
(Trong quá trình phát triển phần mềm, bạn cần phải có tư duy cởi mở và không bao giờ tin tưởng vào một giải pháp là “duy nhất”. Bạn sẽ luôn tìm thấy các tình huống trong đó một công nghệ cụ thể hoạt động tốt hơn một công nghệ khác.)

(continued)
((tiếp theo))

For some of the projects taken individually, you could find one or more alternatives.
(Đối với một số dự án được thực hiện riêng lẻ, bạn có thể tìm thấy một hoặc nhiều lựa chọn thay thế.)

For example, you could choose to use Apache Shiro (https://shiro.apache.org/) instead of Spring Security.
(Ví dụ: bạn có thể chọn sử dụng Apache Shira (https://shiro.apache.org/) thay vì Spring Security.)

Or you could decide to implement your web app using the Play framework (https://www.playframework.com/) instead of Spring MVC and Spring-related technologies.
(Hoặc bạn có thể quyết định triển khai ứng dụng web của mình bằng framework Play (https://www.playframework.com/) thay vì Spring MVC và các công nghệ liên quan đến Spring.)

A more recent project that looks promising is Red Hat Quarkus.
(Một dự án gần đây có vẻ hứa hẹn hơn là Red Hat Quarkus.)

Quarkus is designed for cloud native implementations and becomes more and more mature with rapid steps.
(Quarkus được thiết kế để triển khai trên nền tảng đám mây và ngày càng hoàn thiện hơn với các bước nhanh chóng.)

I wouldn’t be surprised to see it as one of the lead projects in developing enter-prise apps in the Java ecosystem in the future (https://quarkus.io/).
(Tôi sẽ không ngạc nhiên khi coi đây là một trong những dự án hàng đầu trong việc phát triển các ứng dụng dành cho doanh nghiệp trong hệ sinh thái Java trong tương lai (https://quarkus.io/).)

My advice for you is to always take into consideration your alternatives.
(Lời khuyên của tôi dành cho bạn là hãy luôn cân nhắc các lựa chọn thay thế của mình.)

In software development, you need to be open-minded and never trust one solution as being “the one.” You’ll always find scenarios in which a specific technology works better than another.
(Trong quá trình phát triển phần mềm, bạn cần phải có tư duy cởi mở và không bao giờ tin tưởng vào một giải pháp là “duy nhất”. Bạn sẽ luôn tìm thấy các tình huống trong đó một công nghệ cụ thể hoạt động tốt hơn một công nghệ khác.)

(continued)
((tiếp theo))

For some of the projects taken individually, you could find one or more alternatives.
(Đối với một số dự án được thực hiện riêng lẻ, bạn có thể tìm thấy một hoặc nhiều lựa chọn thay thế.)

For example, you could choose to use Apache Shiro (https://shiro.apache.org/) instead of Spring Security.
(Ví dụ: bạn có thể chọn sử dụng Apache Shira (https://shiro.apache.org/) thay vì Spring Security.)

Or you could decide to implement your web app using the Play framework (https://www.playframework.com/) instead of Spring MVC and Spring-related technologies.
(Hoặc bạn có thể quyết định triển khai ứng dụng web của mình bằng framework Play (https://www.playframework.com/) thay vì Spring MVC và các công nghệ liên quan đến Spring.)

A more recent project that looks promising is Red Hat Quarkus.
(Một dự án gần đây có vẻ hứa hẹn hơn là Red Hat Quarkus.)

Quarkus is designed for cloud native implementations and becomes more and more mature with rapid steps.
(Quarkus được thiết kế để triển khai trên nền tảng đám mây và ngày càng hoàn thiện hơn với các bước nhanh chóng.)

I wouldn’t be surprised to see it as one of the lead projects in developing enter-prise apps in the Java ecosystem in the future (https://quarkus.io/).
(Tôi sẽ không ngạc nhiên khi coi đây là một trong những dự án hàng đầu trong việc phát triển các ứng dụng dành cho doanh nghiệp trong hệ sinh thái Java trong tương lai (https://quarkus.io/).)

My advice for you is to always take into consideration your alternatives.
(Lời khuyên của tôi dành cho bạn là hãy luôn cân nhắc các lựa chọn thay thế của mình.)

In software development, you need to be open-minded and never trust one solution as being “the one.” You’ll always find scenarios in which a specific technology works better than another.
(Trong quá trình phát triển phần mềm, bạn cần phải có tư duy cởi mở và không bao giờ tin tưởng vào một giải pháp là “duy nhất”. Bạn sẽ luôn tìm thấy các tình huống trong đó một công nghệ cụ thể hoạt động tốt hơn một công nghệ khác.)

## Spring In Real-World Scenarios

Now that you have an overview of Spring, you’re aware of when and why you should use a framework.
(Bây giờ bạn đã có cái nhìn tổng quan về Spring, bạn đã biết khi nào và tại sao bạn nên sử dụng một framework.)

In this section, I’ll give you some application scenarios in which using the Spring framework might be an excellent fit.
(Trong phần này, tôi sẽ cung cấp cho bạn một số kịch bản ứng dụng trong đó việc sử dụng Spring framework có thể rất phù hợp.)

Too often, I’ve seen developers only refer to backend applications for using a framework like Spring.
(Thông thường, tôi thấy các nhà phát triển chỉ đề cập đến các ứng dụng phụ trợ để sử dụng một framework như Spring.)

I’ve even seen a trend of restricting, even more, the scenario to backend web applications.
(Tôi thậm chí còn nhận thấy xu hướng hạn chế, thậm chí nhiều hơn, kịch bản phụ trợ các ứng dụng web.)

While it’s true that in plenty of cases we see Spring used in this way, it’s important to remember that the framework isn’t limited to this scenario.
(Mặc dù đúng là trong nhiều trường hợp chúng ta thấy Spring được sử dụng theo cách này, nhưng điều quan trọng cần nhớ là framework không bị giới hạn trong trường hợp này.)

I’ve seen teams successfully using Spring in different kinds of applications, such as the development of an automation testing app or even in standalone desktop scenarios.
(Tôi đã thấy các nhóm sử dụng thành công Spring trong nhiều loại ứng dụng khác nhau, chẳng hạn như phát triển ứng dụng thử nghiệm tự động hóa hoặc thậm chí trong các tình huống máy tính để bàn độc lập.)

I’ll further describe to you some common real-world scenarios in which I’ve seen Spring used successfully.
(Tôi sẽ mô tả thêm cho bạn một số tình huống thực tế phổ biến mà tôi đã thấy Spring được sử dụng thành công.)

These are not the only possible scenarios, and Spring might not work all the time in these cases.
(Đây không phải là tình huống duy nhất có thể xảy ra và Spring có thể không hoạt động mọi lúc trong những trường hợp này.)

Remember what we discussed in section 1.2: a framework is not always a good choice.
(Hãy nhớ những gì chúng ta đã thảo luận trong phần 1.2: một framework không phải lúc nào cũng là một lựa chọn tốt.)

But these are common cases in which gener-ally Spring is a good fit:
(Nhưng đây là những trường hợp phổ biến trong đó Spring nói chung là phù hợp:)

1 The development of a backend app
(1 Phát triển ứng dụng phụ trợ)

2 The development of an automation testing framework
(2 Sự phát triển của framework thử nghiệm tự động hóa)

3 The development of a desktop app
(3 Phát triển ứng dụng dành cho máy tính để bàn)

4 The development of a mobile app
(4 Phát triển ứng dụng di động)

### Using Spring In The Development Of A Backend App

A backend application is the part of a system that executes on the server side and has the responsibility of managing data and serving client applications’ requests.
(Ứng dụng phụ trợ là một phần của hệ thống thực thi ở phía máy chủ và có trách nhiệm quản lý dữ liệu cũng như phục vụ các yêu cầu của ứng dụng khách.)

The users access functionalities by using the client apps directly.
(Người dùng truy cập các chức năng bằng cách sử dụng trực tiếp các ứng dụng khách.)

Further, the client apps make requests to the backend app to work with the users’ data.
(Hơn nữa, các ứng dụng khách sẽ yêu cầu ứng dụng phụ trợ hoạt động với dữ liệu của người dùng.)

The backend app
(Ứng dụng phụ trợ)

might use databases to store data or communicate with other backend apps in differ-ent fashions.
(có thể sử dụng cơ sở dữ liệu để lưu trữ dữ liệu hoặc liên lạc với các ứng dụng phụ trợ khác theo các kiểu khác nhau.)

You can imagine, in a real-world scenario, that the app would be the backend application managing the transactions in your bank accounts.
(Bạn có thể tưởng tượng, trong kịch bản thực tế, ứng dụng này sẽ là ứng dụng phụ trợ quản lý các giao dịch trong tài khoản ngân hàng của bạn.)

Users may access their accounts and manage them via a web application (online banking) or a mobile app.
(Người dùng có thể truy cập tài khoản của mình và quản lý chúng thông qua ứng dụng web (ngân hàng trực tuyến) hoặc ứng dụng di động.)

Both the mobile apps and the web apps represent clients for the backend application.
(Cả ứng dụng di động và ứng dụng web đều đại diện cho ứng dụng khách của ứng dụng phụ trợ.)

To manage users’ transactions, the backend application needs to communicate with other backend solutions, and part of the data it manages needs to be persisted in a database.
(Để quản lý các giao dịch của người dùng, ứng dụng phụ trợ cần liên lạc với các giải pháp phụ trợ khác và một phần dữ liệu mà nó quản lý cần phải được lưu giữ trong cơ sở dữ liệu.)

In figure 1.5, you can visualize the architecture of such a system.
(Trong hình 1.5, bạn có thể hình dung kiến ​​trúc của một hệ thống như vậy.)

The users interact with the
(Người dùng tương tác với)

client apps to manage their data.
(ứng dụng khách để quản lý dữ liệu của họ.)

Other backend solutions make direct requests to your backend app.
(Các giải pháp phụ trợ khác đưa ra yêu cầu trực tiếp tới ứng dụng phụ trợ của bạn.)

Your backend app directly communicates with other backend solutions.
(Ứng dụng phụ trợ của bạn giao tiếp trực tiếp với các giải pháp phụ trợ khác.)

The client app make requests to your backend app to resolve users’ requests.
(Ứng dụng khách đưa ra yêu cầu tới ứng dụng phụ trợ của bạn để giải quyết yêu cầu của người dùng.)

Your backend app uses a message broker and adds messages in a queue or topic.
(Ứng dụng phụ trợ của bạn sử dụng trình trung chuyển tin nhắn và thêm tin nhắn vào hàng đợi hoặc chủ đề.)

**Figure 1.5 A backend app interacts in several ways with other apps and uses databases to manage data. Usually, a backend app is complex and may require the use of various technologies. Frameworks simplify the implementation by providing tools you can use to implement the backend solution faster.**
(Hình 1.5 Ứng dụng phụ trợ tương tác theo nhiều cách với các ứng dụng khác và sử dụng cơ sở dữ liệu để quản lý dữ liệu. Thông thường, một ứng dụng phụ trợ rất phức tạp và có thể yêu cầu sử dụng nhiều công nghệ khác nhau. Các framework đơn giản hóa việc triển khai bằng cách cung cấp các công cụ mà bạn có thể sử dụng để triển khai giải pháp phụ trợ nhanh hơn.)

NOTE Don’t worry if you don’t understand all the details of figure 1.5.
(LƯU Ý Đừng lo lắng nếu bạn không hiểu tất cả các chi tiết của hình 1.5.)

I don’t expect you to know what a message broker is and not even how to establish the data exchange among the components.
(Tôi không mong bạn biết nhà môi giới tin nhắn là gì và thậm chí không biết cách thiết lập trao đổi dữ liệu giữa các thành phần.)

What I want you to see is that such a system can become complex in the real world and then understand that projects from the Spring ecosystem were built to help you eliminate this complexity as much as possible.
(Điều tôi muốn bạn thấy là một hệ thống như vậy có thể trở nên phức tạp trong thế giới thực và sau đó hiểu rằng các dự án từ hệ sinh thái Spring được xây dựng để giúp bạn loại bỏ sự phức tạp này nhiều nhất có thể.)

Spring offers an excellent set of tools for implementing backend applications.
(Spring cung cấp một bộ công cụ tuyệt vời để triển khai các ứng dụng phụ trợ.)

It makes your life easier with the different functionalities you generally implement in a backend solution, from integration with other apps to persistence in various database technologies.
(Nó giúp cuộc sống của bạn dễ dàng hơn với các chức năng khác nhau mà bạn thường triển khai trong giải pháp phụ trợ, từ tích hợp với các ứng dụng khác đến tính bền vững trong các công nghệ cơ sở dữ liệu khác nhau.)

It’s no wonder developers often use Spring for such applications.
(Không có gì ngạc nhiên khi các nhà phát triển thường sử dụng Spring cho những ứng dụng như vậy.)

The
(các)

framework basically offers you everything you need in such implementations and is an excellent fit for any kind of architectural style.
(framework về cơ bản cung cấp cho bạn mọi thứ bạn cần trong quá trình triển khai như vậy và rất phù hợp với bất kỳ loại phong cách kiến ​​trúc nào.)

Figure 1.6 indicates the possibilities of using Spring for a backend app.
(Hình 1.6 chỉ ra khả năng sử dụng Spring cho ứng dụng phụ trợ.)

Use the Spring IoC container to manage object instances easier and glue in other functionalities Spring provides.
(Sử dụng bộ chứa Spring IoC để quản lý các phiên bản đối tượng dễ dàng hơn và kết hợp các chức năng khác mà Spring cung cấp.)

Use Spring MVC or Spring WebFlux to implement the REST endpoints called by the client apps or other backend solutions.
(Sử dụng Spring MVC hoặc Spring WebFlux để triển khai các điểm cuối REST được ứng dụng khách hoặc các giải pháp phụ trợ khác gọi.)

Use Spring Security to implement the authentication and authorization configurations.
(Sử dụng Spring Security để triển khai cấu hình xác thực và ủy quyền.)

Use Spring Data to connect to the SQL and NoSQL databases your backend app uses to persist the data.
(Sử dụng Spring Data để kết nối với cơ sở dữ liệu SQL và NoSQL mà ứng dụng phụ trợ của bạn sử dụng để duy trì dữ liệu.)

Use Spring Boot to ease the complexity of your configurations and write less code to implement the app.
(Sử dụng Spring Boot để giảm bớt độ phức tạp trong cấu hình của bạn và viết ít mã hơn để triển khai ứng dụng.)

Use Spring Integration or Spring for Apache Kafka to more easily send messages to your JMS or Kafka topics.
(Sử dụng Spring Integration hoặc Spring for Apache Kafka để gửi tin nhắn đến các chủ đề JMS hoặc Kafka của bạn dễ dàng hơn.)

**Figure 1.6 The possibilities of using Spring in a backend application are endless, from exposing functionalities that other applications can call to managing the database access, and from securing the application to managing integration though third-party message brokers.**
(Hình 1.6 Khả năng sử dụng Spring trong một ứng dụng phụ trợ là vô tận, từ việc hiển thị các chức năng mà các ứng dụng khác có thể gọi đến việc quản lý quyền truy cập cơ sở dữ liệu và từ việc bảo mật ứng dụng đến quản lý tích hợp thông qua các nhà môi giới tin nhắn của bên thứ ba.)

### Using Spring In An Automation Test App

Nowadays, we often use automation testing for end-to-end testing of systems we implement.
(Ngày nay, chúng tôi thường sử dụng thử nghiệm tự động hóa để thử nghiệm từ đầu đến cuối các hệ thống mà chúng tôi triển khai.)

Automation testing refers to implementing software that development teams use to make sure an application behaves as expected.
(Kiểm thử tự động đề cập đến việc triển khai phần mềm mà nhóm phát triển sử dụng để đảm bảo ứng dụng hoạt động như mong đợi.)

A development team can schedule the automation testing implementation to frequently test the app and notify the developers if something is wrong.
(Nhóm phát triển có thể lên lịch triển khai thử nghiệm tự động hóa để thường xuyên kiểm tra ứng dụng và thông báo cho nhà phát triển nếu có sự cố.)

Having such functionality gives developers confidence because they know they’ll be notified if they break anything in the existing capabilities of the app while developing new features.
(Việc có chức năng như vậy mang lại sự tự tin cho các nhà phát triển vì họ biết rằng họ sẽ được thông báo nếu vi phạm bất kỳ điều gì trong khả năng hiện có của ứng dụng trong khi phát triển các tính năng mới.)

While with small systems you can do the testing manually, it’s always a good idea to automate the test cases.
(Mặc dù với các hệ thống nhỏ, bạn có thể thực hiện kiểm thử theo cách thủ công, nhưng việc tự động hóa các trường hợp kiểm thử luôn là một ý tưởng hay.)

For more complex systems, manually testing all the flows isn’t even an option.
(Đối với các hệ thống phức tạp hơn, việc kiểm tra thủ công tất cả các luồng thậm chí không phải là một lựa chọn.)

Because the flows are so numerous, it’d require a massive number of hours and too much energy to cover it completely.
(Bởi vì các dòng chảy rất nhiều nên cần rất nhiều giờ và quá nhiều năng lượng để bao phủ hoàn toàn.)

It turns out that the most efficient solution is to have a separate team implement an app that has the responsibility of validating all the flows of the tested system.
(Hóa ra giải pháp hiệu quả nhất là nhờ một nhóm riêng biệt triển khai một ứng dụng có trách nhiệm xác thực tất cả các luồng của hệ thống đã được thử nghiệm.)

While developers add new functionalities to the system, this testing app is also enhanced to cover what’s new, and the teams use it to validate that everything still works as desired.
(Trong khi các nhà phát triển thêm các chức năng mới vào hệ thống, ứng dụng thử nghiệm này cũng được cải tiến để bao gồm những tính năng mới và các nhóm sử dụng nó để xác thực rằng mọi thứ vẫn hoạt động như mong muốn.)

The developers eventually use an integration tool and schedule the app to run regu-larly to get feedback as soon as possible for their changes (figure 1.7).
(Cuối cùng, các nhà phát triển sử dụng một công cụ tích hợp và lên lịch chạy ứng dụng thường xuyên để nhận phản hồi sớm nhất có thể về những thay đổi của họ (hình 1.7).)

The team continuously adds new tests to cover all the flows developed in the system.
(Nhóm liên tục bổ sung các thử nghiệm mới để bao quát tất cả các luồng được phát triển trong hệ thống.)

Usually, the app is stored in a repository of a version management system like Git.
(Thông thường, ứng dụng được lưu trữ trong kho lưu trữ của hệ thống quản lý phiên bản như Git.)

A continuous integration tool like Jenkins regularly runs all the tests.
(Một công cụ tích hợp liên tục như Jenkins thường xuyên chạy tất cả các bài kiểm thử.)

If a test is failing,
(Nếu một bài kiểm tra thất bại,)

Jenkins notifies the team.
(Jenkins thông báo cho nhóm.)

**Figure 1.7 The team deploys the testing app in a test environment. A continuous integration tool like Jenkins executes the app regularly and sends feedback to the team. This way, the team is always aware of the system’s status, and they know if they break something during development.**
(Hình 1.7 Nhóm triển khai ứng dụng thử nghiệm trong môi trường thử nghiệm. Một công cụ tích hợp liên tục như Jenkins thực thi ứng dụng thường xuyên và gửi phản hồi cho nhóm. Bằng cách này, nhóm luôn biết được trạng thái của hệ thống và họ biết liệu mình có làm hỏng thứ gì đó trong quá trình phát triển hay không.)

Such an application might become as complex as a backend app.
(Một ứng dụng như vậy có thể trở nên phức tạp như một ứng dụng phụ trợ.)

In order to validate the flows, the app needs to communicate with the components of the system and even connect to databases.
(Để xác thực các luồng, ứng dụng cần giao tiếp với các thành phần của hệ thống và thậm chí kết nối với cơ sở dữ liệu.)

Sometimes the app mocks external dependencies to simulate different execution scenarios.
(Đôi khi ứng dụng mô phỏng các phần phụ thuộc bên ngoài để mô phỏng các tình huống thực thi khác nhau.)

For writing the test scenarios, developers use frameworks like Selenium, Cucumber, Gauge, and others.
(Để viết các kịch bản thử nghiệm, các nhà phát triển sử dụng các framework như Selenium, Cucumber, Gauge và các framework khác.)

But, together with these frameworks, the app could still benefit in several ways from Spring’s tools.
(Tuy nhiên, cùng với các framework này, ứng dụng vẫn có thể hưởng lợi từ các công cụ của Spring theo một số cách.)

For example, the app could manage the object instances to make the code more maintainable using the Spring IoC container.
(Ví dụ: ứng dụng có thể quản lý các phiên bản đối tượng để làm cho mã dễ bảo trì hơn bằng cách sử dụng bộ chứa Spring IoC.)

It could use Spring Data to connect to the databases where it needs to validate the data.
(Nó có thể sử dụng Spring Data để kết nối với cơ sở dữ liệu cần xác thực dữ liệu.)

It could send messages to queues or topics of a broker system to simulate specific scenarios or simply use Spring to call some REST endpoints (figure 1.8).
(Nó có thể gửi tin nhắn đến hàng đợi hoặc chủ đề của hệ thống môi giới để mô phỏng các kịch bản cụ thể hoặc đơn giản sử dụng Spring để gọi một số điểm cuối REST (hình 1.8).)

(Remember, it’s okay if this looks too advanced; meaning will be clarified as you progress through the book).
((Hãy nhớ rằng, điều này có vẻ quá cao cấp cũng không sao; ý nghĩa sẽ được làm rõ khi bạn đọc hết cuốn sách).)

The testing app may use Spring MVC to simulate calls from other systems.
(Ứng dụng thử nghiệm có thể sử dụng Spring MVC để mô phỏng cuộc gọi từ các hệ thống khác.)

The testing app may use Spring Data to connect to the SQL and NoSQL database your backend app uses to persist the data.
(Ứng dụng thử nghiệm có thể sử dụng Spring Data để kết nối với cơ sở dữ liệu SQL và NoSQL mà ứng dụng phụ trợ của bạn sử dụng để duy trì dữ liệu.)

The testing app may use Spring Integration to send messages to queues or topics.
(Ứng dụng thử nghiệm có thể sử dụng Spring Integration để gửi tin nhắn đến hàng đợi hoặc chủ đề.)

**Figure 1.8 A testing app might need to connect to databases or communicate with other systems or the tested system. The developers can use components of the Spring ecosystem to simplify the implementations of these functionalities.**
(Hình 1.8 Ứng dụng thử nghiệm có thể cần kết nối với cơ sở dữ liệu hoặc liên lạc với các hệ thống khác hoặc hệ thống được thử nghiệm. Các nhà phát triển có thể sử dụng các thành phần của hệ sinh thái Spring để đơn giản hóa việc triển khai các chức năng này.)

### Using Spring For The Development Of A Desktop App

Today, desktop applications are not that frequently developed, as web or mobile apps have taken the role of interacting with the user.
(Ngày nay, các ứng dụng dành cho máy tính để bàn không được phát triển thường xuyên vì các ứng dụng web hoặc thiết bị di động đã đóng vai trò tương tác với người dùng.)

However, there’s still a small number of desktop applications, and components of the Spring ecosystem could be a good choice in the development of their features.
(Tuy nhiên, vẫn còn một số lượng nhỏ ứng dụng dành cho máy tính để bàn và các thành phần của hệ sinh thái Spring có thể là một lựa chọn tốt trong việc phát triển các tính năng của chúng.)

A desktop app could successfully use the Spring IoC container to manage the object instances.
(Một ứng dụng dành cho máy tính để bàn có thể sử dụng thành công bộ chứa Spring IoC để quản lý các phiên bản đối tượng.)

This way, the app’s implementa-tion is cleaner and improves its maintainability.
(Bằng cách này, quá trình triển khai ứng dụng sẽ rõ ràng hơn và cải thiện khả năng bảo trì của ứng dụng.)

Additionally, the app could potentially use Spring’s tools to implement different features, for example to communicate with a backend or other components (calling web services or using other techniques for remote calls) or implement a caching solution.
(Ngoài ra, ứng dụng có thể sử dụng các công cụ của Spring để triển khai các tính năng khác nhau, chẳng hạn như để giao tiếp với phần phụ trợ hoặc các thành phần khác (gọi dịch vụ web hoặc sử dụng các kỹ thuật khác cho cuộc gọi từ xa) hoặc triển khai giải pháp bộ nhớ đệm.)

### Using Spring In Mobile Apps

With its Spring for Android project (https://spring.io/projects/spring-android), the Spring community tries to help the development of mobile applications.
(Với dự án Spring dành cho Android (https://spring.io/projects/spring-android), cộng đồng Spring cố gắng hỗ trợ việc phát triển các ứng dụng di động.)

Even though you’ll probably rarely encounter this situation, it’s worth mentioning that you can use Spring’s tools to develop Android apps.
(Mặc dù có thể bạn sẽ hiếm khi gặp phải tình huống này nhưng điều đáng nói là bạn có thể sử dụng các công cụ của Spring để phát triển ứng dụng Android.)

This Spring project provides a REST client for Android and authentication support for accessing secured APIs.
(Dự án Spring này cung cấp ứng dụng khách REST cho Android và hỗ trợ xác thực để truy cập các API được bảo mật.)

## When Not To Use Frameworks

In this section, we discuss why you should sometimes avoid using frameworks.
(Trong phần này, chúng tôi thảo luận lý do tại sao đôi khi bạn nên tránh sử dụng các framework.)

It’s essential you know when to use a framework and when to avoid using them.
(Điều cần thiết là bạn phải biết khi nào nên sử dụng một framework và khi nào nên tránh sử dụng chúng.)

Some-times, using a tool that’s too much for the job might consume more energy and also obtain a worse result.
(Đôi khi, việc sử dụng một công cụ quá sức cho công việc có thể tiêu tốn nhiều năng lượng hơn và cũng mang lại kết quả tồi tệ hơn.)

Imagine using a chainsaw to cut bread.
(Hãy tưởng tượng bạn sử dụng cưa máy để cắt bánh mì.)

While you could try to and even achieve a final result, it’d be more difficult and energy-consuming than using a regular knife (and you may end up with nothing but breadcrumbs instead of sliced bread).
(Mặc dù bạn có thể cố gắng và thậm chí đạt được kết quả cuối cùng, nhưng việc này sẽ khó khăn và tốn nhiều năng lượng hơn so với việc sử dụng một con dao thông thường (và bạn có thể không nhận được gì ngoài vụn bánh mì thay vì bánh mì cắt lát).)

We’ll discuss a few scenarios in which using a framework isn’t a great idea, and then I’ll tell you a story about a team I was part of that failed in the implementation of an app because of using a framework.
(Chúng ta sẽ thảo luận về một số tình huống trong đó việc sử dụng framework không phải là một ý tưởng hay và sau đó tôi sẽ kể cho bạn câu chuyện về một nhóm mà tôi tham gia đã thất bại trong việc triển khai ứng dụng do sử dụng framework.)

It turns out that, like everything else in software development, you shouldn’t apply a framework in all cases.
(Hóa ra, giống như mọi thứ khác trong phát triển phần mềm, bạn không nên áp dụng một khuôn khổ nào đó trong mọi trường hợp.)

You’ll find situations in which a framework is not a good fit—or maybe a framework is a good fit, but not the Spring framework.
(Bạn sẽ tìm thấy các tình huống trong đó một framework không phù hợp—hoặc có thể một framework phù hợp nhưng không phù hợp với framework Spring.)

In which of the fol-lowing scenarios should you consider not using a framework?
(Bạn nên cân nhắc việc không sử dụng framework trong trường hợp nào sau đây?)

1 You need to implement a particular functionality with a footprint as small as possible.
(1 Bạn cần triển khai một chức năng cụ thể với dung lượng nhỏ nhất có thể.)

By footprint, I mean the storage memory occupied by the app’s files.
(Theo dấu chân, ý tôi là bộ nhớ lưu trữ bị chiếm bởi các tệp của ứng dụng.)

2 Specific security requirements force you to implement only custom code in your app without making use of any open source framework.
(2 Các yêu cầu bảo mật cụ thể buộc bạn chỉ triển khai mã tùy chỉnh trong ứng dụng của mình mà không sử dụng bất kỳ framework nguồn mở nào.)

3 You’d have to make so many customizations over the framework that you’d write more code than if you’d simply not used it at all.
(3 Bạn sẽ phải thực hiện nhiều tùy chỉnh trên framework đến mức bạn sẽ viết nhiều mã hơn so với khi bạn hoàn toàn không sử dụng nó.)

4 You already have a functional app, and by changing it to use a framework you don’t gain any benefit.
(4 Bạn đã có một ứng dụng chức năng và bằng cách thay đổi nó để sử dụng một framework, bạn sẽ không thu được bất kỳ lợi ích nào.)

Let’s discuss these points in more detail.
(Hãy thảo luận về những điểm này chi tiết hơn.)

### You Need To Have A Small Footprint

For point one, I refer to situations in which you need to make your application small.
(Đối với điểm một, tôi đề cập đến các tình huống mà bạn cần làm cho ứng dụng của mình trở nên nhỏ gọn.)

In today’s systems, we find more and more cases in which the services are delivered in containers.
(Trong các hệ thống ngày nay, chúng ta thấy ngày càng nhiều trường hợp dịch vụ được cung cấp trong container.)

You’ve likely heard about containers, such as Docker, Kubernetes, or other terms related to this subject (if not, again, that’s okay).
(Bạn có thể đã nghe nói về các container, chẳng hạn như Docker, Kubernetes hoặc các thuật ngữ khác liên quan đến chủ đề này (nếu không thì cũng không sao).)

Containers in their entirety is a topic beyond the scope of this book, so for now the only thing I need you to know is that when you use such a deployment fashion, you want your application to be as small as possible.
(Toàn bộ vùng chứa là một chủ đề nằm ngoài phạm vi của cuốn sách này, vì vậy bây giờ điều duy nhất tôi cần bạn biết là khi bạn sử dụng kiểu triển khai như vậy, bạn muốn ứng dụng của mình càng nhỏ càng tốt.)

A container is like a box in which your application lives.
(Vùng chứa giống như một chiếc hộp chứa ứng dụng của bạn.)

One crucial principle regarding app deployment in containers is that the containers should be easily disposable: they can be destroyed and recreated as fast as possible.
(Một nguyên tắc quan trọng liên quan đến việc triển khai ứng dụng trong vùng chứa là vùng chứa phải dễ dàng sử dụng một lần: chúng có thể bị phá hủy và tạo lại nhanh nhất có thể.)

The size of the app (footprint) matters a lot here.
(Kích thước của ứng dụng (dấu chân) rất quan trọng ở đây.)

You can save sec-onds from the app initialization by making it smaller.
(Bạn có thể tiết kiệm vài giây khi khởi chạy ứng dụng bằng cách làm cho nó nhỏ hơn.)

That doesn’t mean you won’t use frameworks for all the apps deployed in containers.
(Điều đó không có nghĩa là bạn sẽ không sử dụng framework cho tất cả ứng dụng được triển khai trong vùng chứa.)

But for some apps, which are usually also quite small, it makes more sense to improve their initialization and make their footprint smaller rather than adding depen-dencies to different frameworks.
(Nhưng đối với một số ứng dụng, thường cũng khá nhỏ, sẽ hợp lý hơn nếu cải thiện quá trình khởi tạo và làm cho dấu chân của chúng nhỏ hơn thay vì thêm các phần phụ thuộc vào các framework khác nhau.)

Such a case is a kind of application called server-less function.
(Trường hợp như vậy là một loại ứng dụng được gọi là chức năng không có máy chủ.)

These server-less functions are tiny applications deployed in containers.
(Các chức năng không có máy chủ này là các ứng dụng nhỏ được triển khai trong các vùng chứa.)

Because you don’t have too much access to the way they’re deployed, it looks like they execute without a server (hence their name).
(Vì bạn không có quá nhiều quyền truy cập vào cách chúng được triển khai nên có vẻ như chúng thực thi mà không cần máy chủ (do đó có tên như vậy).)

These apps need to be small, and that’s why, for this specific case of apps, you’ll want to avoid adding a framework as much as possible.
(Các ứng dụng này cần phải nhỏ và đó là lý do tại sao, đối với trường hợp ứng dụng cụ thể này, bạn sẽ muốn tránh thêm framework càng nhiều càng tốt.)

Because of its size, it’s also possible that you won’t need a framework anyway.
(Vì kích thước của nó nên cũng có thể bạn sẽ không cần đến framework.)

### Security Needs Dictate Custom Code

I said in point two that in specific situations, apps could not use frameworks because of security requirements.
(Tôi đã nói ở điểm thứ hai rằng trong các tình huống cụ thể, ứng dụng không thể sử dụng framework vì yêu cầu bảo mật.)

This scenario usually happens with apps in the field of defense or governmental organizations.
(Tình huống này thường xảy ra với các ứng dụng trong lĩnh vực quốc phòng hoặc tổ chức chính phủ.)

Again, it doesn’t mean all the apps used in governmental organizations are prohibited from using frameworks, but for some, restrictions are applied.
(Một lần nữa, điều đó không có nghĩa là tất cả các ứng dụng được sử dụng trong các tổ chức chính phủ đều bị cấm sử dụng các khuôn khổ, nhưng đối với một số ứng dụng, các hạn chế vẫn được áp dụng.)

You may wonder why.
(Bạn có thể thắc mắc tại sao.)

Well, say an open source framework like Spring is used.
(Vâng, giả sử một framework nguồn mở như Spring được sử dụng.)

If someone finds a specific vulnerability, it will become known, and a hacker could use this knowledge to exploit it.
(Nếu ai đó tìm thấy một lỗ hổng cụ thể, lỗ hổng đó sẽ được biết đến và tin tặc có thể sử dụng kiến ​​thức này để khai thác nó.)

Sometimes, stakeholders of such apps want to make sure the chances of someone hacking into their system is as close to zero as possible.
(Đôi khi, các bên liên quan của những ứng dụng như vậy muốn đảm bảo khả năng ai đó xâm nhập vào hệ thống của họ càng gần bằng 0 càng tốt.)

This could lead to even rebuilding a functionality instead of using it from a third-party source.
(Điều này thậm chí có thể dẫn đến việc xây dựng lại một chức năng thay vì sử dụng nó từ nguồn của bên thứ ba.)

NOTE Wait!
(LƯU Ý Đợi đã!)

Earlier I said that it’s more secure to use an open source framework because if a vulnerability exists, someone will likely discover it.
(Trước đó tôi đã nói rằng sẽ an toàn hơn khi sử dụng framework nguồn mở vì nếu có lỗ hổng bảo mật thì ai đó có thể sẽ phát hiện ra nó.)

Well, if you invest enough time and money, you probably can achieve this yourself as well.
(Chà, nếu bạn đầu tư đủ thời gian và tiền bạc, có lẽ bạn cũng có thể tự mình đạt được điều này.)

In general, it’s cheaper to use a framework, of course.
(Nói chung, tất nhiên là rẻ hơn khi sử dụng một framework.)

And if you don’t want to be extra cautious, it makes more sense to use a framework.
(Và nếu bạn không muốn thận trọng hơn thì việc sử dụng một framework sẽ hợp lý hơn.)

But in some projects, the stakeholders really want to make sure no information becomes public.
(Nhưng trong một số dự án, các bên liên quan thực sự muốn đảm bảo rằng không có thông tin nào được công khai.)

### Abundant Existing Customizations Make A Framework Impractical

Another case (point three) in which you might want to avoid using a framework is when you’d have to customize its components so much that you end up writing more code than if it hadn’t been used.
(Một trường hợp khác (điểm thứ ba) mà bạn có thể muốn tránh sử dụng một framework là khi bạn phải tùy chỉnh các thành phần của nó nhiều đến mức cuối cùng bạn phải viết nhiều mã hơn so với khi nó chưa được sử dụng.)

As I specified in section 1.1, a framework provides you parts that you assemble with your business code to obtain an app.
(Như tôi đã chỉ định trong phần 1.1, một framework cung cấp cho bạn các bộ phận mà bạn lắp ráp với mã doanh nghiệp của mình để có được một ứng dụng.)

These compo-nents, provided by the framework, don’t fit perfectly, and you need to customize them in different ways.
(Các thành phần này do framework cung cấp không hoàn toàn phù hợp và bạn cần tùy chỉnh chúng theo nhiều cách khác nhau.)

It’s perfectly normal to customize the framework’s components and the style in which they assemble than if you’d developed the functionality from scratch.
(Việc tùy chỉnh các thành phần của framework và kiểu lắp ráp của chúng là điều hoàn toàn bình thường so với việc bạn phát triển chức năng này từ đầu.)

If you find yourself in such a situation, you have probably chosen the wrong framework (search for alternatives) or you shouldn’t use a framework at all.
(Nếu bạn rơi vào tình huống như vậy thì có thể bạn đã chọn sai framework (tìm kiếm giải pháp thay thế) hoặc bạn hoàn toàn không nên sử dụng một framework nào cả.)

You won’t benefit from switching to a framework
(Bạn sẽ không được hưởng lợi từ việc chuyển sang một framework)

In point four, I mentioned that a potential mistake could be trying to use a framework to replace something that already exists and is working in an app.
(Ở điểm thứ tư, tôi đã đề cập rằng một lỗi tiềm ẩn có thể là cố gắng sử dụng một framework để thay thế thứ gì đó đã tồn tại và đang hoạt động trong một ứng dụng.)

Sometimes we are tempted to replace an existing architecture with something new.
(Đôi khi chúng ta bị cám dỗ thay thế kiến ​​trúc hiện tại bằng một kiến ​​trúc mới.)

A new framework appears, and it’s popular, and everyone uses it, so why shouldn’t we change our app as well to use this framework?
(Một framework mới xuất hiện, nó phổ biến và mọi người đều sử dụng nó, vậy tại sao chúng ta không thay đổi ứng dụng của mình để sử dụng framework này?)

You can, but you need to attentively analyze what you want to achieve by changing something that works.
(Bạn có thể, nhưng bạn cần phân tích kỹ lưỡng những gì bạn muốn đạt được bằng cách thay đổi điều gì đó có hiệu quả.)

In some cases, like my story from section
(Trong một số trường hợp, như câu chuyện của tôi ở phần)

1.1, it could be helpful to change your app and make it rely on a specific framework.
(1.1, việc thay đổi ứng dụng của bạn và làm cho ứng dụng dựa vào một framework cụ thể có thể sẽ hữu ích.)

As long as this change brings a benefit, do it!
(Chỉ cần sự thay đổi này mang lại lợi ích thì hãy thực hiện!)

A reason could be that you want to make the app more maintainable, more performant, or more secure.
(Lý do có thể là bạn muốn làm cho ứng dụng dễ bảo trì hơn, hiệu suất cao hơn hoặc an toàn hơn.)

But if this change doesn’t bring you a benefit, and sometimes it might even bring incertitude, then, in the end, you might discover you invested the time and money for a worse result.
(Nhưng nếu sự thay đổi này không mang lại lợi ích cho bạn và đôi khi nó thậm chí có thể mang lại sự thiếu chắc chắn, thì cuối cùng, bạn có thể phát hiện ra rằng mình đã đầu tư thời gian và tiền bạc để đạt được kết quả tồi tệ hơn.)

Let me tell you a story from my own experience.
(Hãy để tôi kể cho bạn một câu chuyện từ kinh nghiệm của chính tôi.)

### An Avoidable Mistake

Using frameworks isn’t always the best choice, and I had to learn that the hard way.
(Sử dụng các framework không phải lúc nào cũng là lựa chọn tốt nhất và tôi đã phải học điều đó một cách khó khăn.)

Years earlier, we were working on the backend of a web application.
(Nhiều năm trước, chúng tôi đang làm việc ở phần phụ trợ của một ứng dụng web.)

Times influence many things, including software architectures.
(Thời gian ảnh hưởng đến nhiều thứ, bao gồm cả kiến ​​trúc phần mềm.)

The app was using JDBC to directly connect to an Oracle database.
(Ứng dụng đang sử dụng JDBC để kết nối trực tiếp với cơ sở dữ liệu Oracle.)

The code was quite ugly.
(Mã này khá xấu.)

Everywhere the app needed to execute a query on the database it opened a statement and then sent a query that was sometimes written on multiple rows.
(Ở mọi nơi ứng dụng cần thực hiện một truy vấn trên cơ sở dữ liệu, nó sẽ mở một câu lệnh và sau đó gửi một truy vấn đôi khi được viết trên nhiều hàng.)

You might be young enough not to have encountered JDBC direct usage in apps, but trust me, it’s a long and ugly code.
(Bạn có thể còn trẻ để chưa gặp phải việc sử dụng trực tiếp JDBC trong các ứng dụng, nhưng hãy tin tôi, đó là một đoạn mã dài và xấu.)

At that time, some frameworks using another methodology to work with the database were becoming more and more popular.
(Vào thời điểm đó, một số framework sử dụng phương pháp khác để làm việc với cơ sở dữ liệu ngày càng trở nên phổ biến.)

I remember when I first encountered Hibernate.
(Tôi nhớ lần đầu tiên tôi gặp Hibernate.)

This is an ORM framework, which allows you to treat the tables and their relationships in a database as objects and relationships among objects.
(Đây là framework ORM, cho phép bạn coi các bảng và mối quan hệ của chúng trong cơ sở dữ liệu dưới dạng đối tượng và mối quan hệ giữa các đối tượng.)

When used correctly, it enables you to write less code and more intuitive functionality.
(Khi được sử dụng đúng cách, nó cho phép bạn viết ít mã hơn và có nhiều chức năng trực quan hơn.)

When misused, it may slow down your app, make the code less intuitive, and even introduce bugs.
(Khi sử dụng sai mục đích, nó có thể làm chậm ứng dụng của bạn, làm cho mã kém trực quan hơn và thậm chí gây ra lỗi.)

The application we were developing needed a change.
(Ứng dụng chúng tôi đang phát triển cần một sự thay đổi.)

We knew we could improve that ugly JDBC code.
(Chúng tôi biết mình có thể cải thiện mã JDBC xấu xí đó.)

In my mind, we could at least minimize the number of lines.
(Trong suy nghĩ của tôi, ít nhất chúng ta có thể giảm thiểu số lượng dòng.)

This change would have brought great benefits to maintainability.
(Sự thay đổi này sẽ mang lại lợi ích to lớn cho khả năng bảo trì.)

Together with other developers, we suggested using a tool provided by Spring called JdbcTemplate (you’ll learn this tool in chapter 12).
(Cùng với các nhà phát triển khác, chúng tôi đề xuất sử dụng một công cụ do Spring cung cấp có tên là JdbcTemplate (bạn sẽ tìm hiểu công cụ này trong chương 12).)

But others strongly pushed the decision to use Hibernate.
(Nhưng những người khác lại thúc đẩy quyết định sử dụng Hibernate một cách mạnh mẽ.)

It was quite popular, so why not to use it?
(Nó khá phổ biến, vậy tại sao không sử dụng nó?)

(Actually it still is one of the most popular frameworks of its kind, and you’ll learn about integrating it with Spring in chapter 13.) I could see changing that code to a completely new methodology would be a challenge.
((Trên thực tế, nó vẫn là một trong những framework phổ biến nhất thuộc loại này và bạn sẽ tìm hiểu về cách tích hợp nó với Spring ở chương 13.) Tôi có thể thấy việc thay đổi mã đó sang một phương pháp hoàn toàn mới sẽ là một thách thức.)

Moreover, I could see no benefits.
(Hơn nữa, tôi không thể thấy được lợi ích gì.)

The change also implied a greater risk of introducing bugs.
(Sự thay đổi này cũng ngụ ý nguy cơ xuất hiện lỗi cao hơn.)

Fortunately, the change started with a proof of concept.
(May mắn thay, sự thay đổi bắt đầu bằng một bằng chứng về khái niệm.)

After a couple of months, lots of effort, and stress, the team decided to quit.
(Sau vài tháng, rất nhiều nỗ lực và căng thẳng, cả nhóm quyết định nghỉ việc.)

After analyzing our options, we finished the implementation using JdbcTemplate.
(Sau khi phân tích các tùy chọn của mình, chúng tôi đã hoàn tất quá trình triển khai bằng JdbcTemplate.)

We managed to write cleaner code by eliminating a large number of lines of code, and we didn’t need to introduce any new framework for this change.
(Chúng tôi đã cố gắng viết mã sạch hơn bằng cách loại bỏ một số lượng lớn dòng mã và chúng tôi không cần giới thiệu bất kỳ khuôn khổ mới nào cho thay đổi này.)

## What Will You Learn In This Book

Since you opened this book, I assume you’re probably a software developer in the Java ecosystem who found out it’s useful to learn Spring.
(Vì bạn đã mở cuốn sách này nên tôi cho rằng bạn có thể là một nhà phát triển phần mềm trong hệ sinh thái Java, người nhận thấy việc học Spring rất hữu ích.)

The purpose of this book is to teach you the foundations of Spring, assuming you know nothing at all about frameworks and, of course, about Spring.
(Mục đích của cuốn sách này là dạy cho bạn những nền tảng của Spring, giả sử bạn không biết gì về framework và tất nhiên là về Spring.)

When I say Spring, I refer to the Spring ecosystem, not just the core part of the framework.
(Khi tôi nói Spring, tôi muốn nói đến hệ sinh thái Spring chứ không chỉ là phần cốt lõi của framework.)

When you finish the book, you will have learned how to do the following:
(Khi đọc xong cuốn sách, bạn sẽ học được cách thực hiện những điều sau:)

Use the Spring context and implement aspects around objects managed by the framework.
(Sử dụng bối cảnh Spring và triển khai các khía cạnh xung quanh các đối tượng do framework quản lý.)

Implement the mechanism of a Spring app to connect to a database and work with the persisted data.
(Triển khai cơ chế của ứng dụng Spring để kết nối với cơ sở dữ liệu và làm việc với dữ liệu lâu dài.)

Establish data exchange between apps using REST APIs implemented with Spring.
(Thiết lập trao đổi dữ liệu giữa các ứng dụng bằng API REST được triển khai với Spring.)

Build basic apps that use the convention-over-configuration approach.
(Xây dựng các ứng dụng cơ bản sử dụng phương pháp cấu hình theo quy ước.)

Use best practices in the standard class design of a Spring application.
(Sử dụng các phương pháp hay nhất trong thiết kế lớp tiêu chuẩn của ứng dụng Spring.)

Properly test your Spring implementations.
(Kiểm tra đúng việc triển khai Spring của bạn.)

## Summary

An application framework is a set of common software functionalities that pro-vides a foundational structure for developing an application.
(Khung ứng dụng là một tập hợp các chức năng phần mềm phổ biến cung cấp cấu trúc nền tảng để phát triển ứng dụng.)

A framework acts as the skeletal support to build an application.
(Một framework hoạt động như bộ framework hỗ trợ để xây dựng một ứng dụng.)

A framework helps you build an app more efficiently by providing functionality that you assemble to your implementation instead of developing it yourself.
(Khung giúp bạn xây dựng ứng dụng hiệu quả hơn bằng cách cung cấp chức năng mà bạn lắp ráp để triển khai thay vì tự phát triển ứng dụng đó.)

Using a framework saves you time and helps ensure there are fewer chances of implementing buggy features.
(Việc sử dụng một framework giúp bạn tiết kiệm thời gian và giúp đảm bảo có ít cơ hội triển khai các tính năng có lỗi hơn.)

Using a widely known framework like Spring opens a door to a large community, which makes it more likely that others will faces similar problems.
(Việc sử dụng một framework được biết đến rộng rãi như Spring sẽ mở ra cánh cửa cho một cộng đồng lớn, điều này khiến nhiều khả năng những người khác sẽ gặp phải những vấn đề tương tự.)

You then have an excellent opportunity to learn about how others solved something similar to an issue you need to address, which will spare you the time of individual research.
(Sau đó, bạn có cơ hội tuyệt vời để tìm hiểu về cách người khác giải quyết vấn đề tương tự như vấn đề bạn cần giải quyết, điều này sẽ giúp bạn tiết kiệm thời gian nghiên cứu cá nhân.)

When implementing an application, always think of all possibilities, including not using a framework.
(Khi triển khai một ứng dụng, hãy luôn nghĩ đến mọi khả năng, kể cả việc không sử dụng framework.)

If you decide to use one or more frameworks, take into consideration all their alternatives.
(Nếu bạn quyết định sử dụng một hoặc nhiều framework, hãy xem xét tất cả các lựa chọn thay thế của chúng.)

You should think about the purpose of the framework, who else is using it (how big the community is), and for how long it’s been on the market (maturity).
(Bạn nên suy nghĩ về mục đích của framework này, ai khác đang sử dụng nó (cộng đồng lớn như thế nào) và nó đã có mặt trên thị trường được bao lâu (sự trưởng thành).)

Spring is not just a framework.
(Mùa xuân không chỉ là một khuôn khổ.)

We often refer to Spring as “Spring framework” to indicate the core functionalities, but Spring offers an entire ecosystem formed of many projects used in application development.
(Chúng ta thường gọi Spring là “Spring framework” để chỉ các chức năng cốt lõi, nhưng Spring cung cấp toàn bộ hệ sinh thái được hình thành từ nhiều dự án được sử dụng trong phát triển ứng dụng.)

Each project is dedi-cated to a specific domain, and when implementing an app, you might use more of these projects to implement the functionality you desire.
(Mỗi dự án được dành riêng cho một miền cụ thể và khi triển khai một ứng dụng, bạn có thể sử dụng nhiều dự án này hơn để triển khai chức năng mà bạn mong muốn.)

The projects of the Spring ecosystem we’ll use in this book are as follows:
(Các dự án của hệ sinh thái Spring mà chúng tôi sẽ sử dụng trong cuốn sách này như sau:)

Spring Core, which builds the foundation of Spring and provides features like the context, aspects, and basic data access.
(Spring Core, xây dựng nền tảng của Spring và cung cấp các tính năng như bối cảnh, các khía cạnh và truy cập dữ liệu cơ bản.)

Spring Data, which provides a high-level, comfortable-to-use set of tools to implement the persistence layer of your apps.
(Spring Data, cung cấp bộ công cụ cấp cao, dễ sử dụng để triển khai lớp lưu giữ lâu dài cho ứng dụng của bạn.)

You’ll find how easy it is to use Spring Data to work with both SQL and NoSQL databases.
(Bạn sẽ thấy việc sử dụng Spring Data để làm việc với cả cơ sở dữ liệu SQL và NoSQL dễ dàng như thế nào.)

Spring Boot, which is a project of the Spring ecosystem that helps you apply a “convention-over-configuration” approach.
(Spring Boot, là một dự án của hệ sinh thái Spring giúp bạn áp dụng cách tiếp cận “convention-over-configuration”.)

Quite often, learning materials (like books, articles, or video tutorials) offer examples with Spring only for backend applications.
(Thông thường, các tài liệu học tập (như sách, bài viết hoặc video hướng dẫn) chỉ cung cấp các ví dụ về Spring cho các ứng dụng phụ trợ.)

While it’s true that it’s widespread to use Spring with backend apps, you can use Spring with other kinds of apps as well, even in desktop applications and automation testing apps.
(Mặc dù đúng là việc sử dụng Spring với các ứng dụng phụ trợ là phổ biến, nhưng bạn cũng có thể sử dụng Spring với các loại ứng dụng khác, ngay cả trong các ứng dụng dành cho máy tính để bàn và ứng dụng thử nghiệm tự động hóa.)

The Spring context: Defining beansThe Spring context: Defining beans
(Bối cảnh mùa xuân: Xác định các loại đậu Bối cảnh mùa xuân: Xác định các loại đậu)

The Spring context: Defining beans
(Bối cảnh mùa xuân: Xác định đậu)

Understanding the need for Spring context
(Hiểu nhu cầu về bối cảnh mùa xuân)

Adding new object instances to the Spring context
(Thêm các phiên bản đối tượng mới vào bối cảnh Spring)

Understanding the need for Spring context
(Hiểu nhu cầu về bối cảnh mùa xuân)

Adding new object instances to the Spring context
(Thêm các phiên bản đối tượng mới vào bối cảnh Spring)

In this chapter, you start learning how to work with a crucial Spring framework ele-ment: the context (also known as the application context in a Spring app).
(Trong chương này, bạn bắt đầu học cách làm việc với một thành phần quan trọng của Spring framework: context (còn được gọi là bối cảnh ứng dụng trong ứng dụng Spring).)

Imagine the context as a place in the memory of your app in which we add all the object instances that we want the framework to manage.
(Hãy tưởng tượng bối cảnh như một vị trí trong bộ nhớ ứng dụng của bạn, trong đó chúng ta thêm tất cả các phiên bản đối tượng mà chúng ta muốn framework quản lý.)

By default, Spring doesn’t know any of the objects you define in your application.
(Theo mặc định, Spring không biết bất kỳ đối tượng nào bạn xác định trong ứng dụng của mình.)

To enable Spring to see your objects, you need to add them to the context.
(Để cho phép Spring xem các đối tượng của bạn, bạn cần thêm chúng vào ngữ cảnh.)

Later in this book we discuss using different capabilities provided by Spring in apps.
(Ở phần sau của cuốn sách này, chúng ta sẽ thảo luận về việc sử dụng các khả năng khác nhau do Spring cung cấp trong ứng dụng.)

You’ll learn that plugging in such features is done through the context by adding object instances and establishing relationships among them.
(Bạn sẽ biết rằng việc cài đặt các tính năng như vậy được thực hiện thông qua ngữ cảnh bằng cách thêm các phiên bản đối tượng và thiết lập mối quan hệ giữa chúng.)

Spring uses the instances in the context to connect your app to various functionalities it provides.
(Spring sử dụng các phiên bản trong ngữ cảnh để kết nối ứng dụng của bạn với các chức năng khác nhau mà nó cung cấp.)

You’ll learn the basics of the most import-ant features (e.g., transactions, testing, etc.) throughout the book.
(Bạn sẽ tìm hiểu những kiến ​​thức cơ bản về những tính năng quan trọng nhất (ví dụ: giao dịch, thử nghiệm, v.v.) trong suốt cuốn sách.)
