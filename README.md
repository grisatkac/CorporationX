# CorporationX

I worked on this project with a team of 5 people. The project was written on a microservice architecture. The following is a description of the implemented features

# My features

## Used Minio (Amazon S3 compatible) to store user image in User Service.
link: https://github.com/CorporationX/user_service/pull/1285/files#diff-38a41377204c067361cfe9ea7cfcacb929d371b2932d2e7bc87185ac621f7f2f

## Integrated Google SMTP into Notification Service.
link: https://github.com/CorporationX/notification_service/blob/notification-service-grisatkac/src/main/java/faang/school/notificationservice/service/notification/EmailService.java

## Used Redis for data caching and publishing, event listener (Pub/Sub).
link: https://github.com/CorporationX/post_service/blob/centaur-master-bc5/src/main/java/faang/school/postservice/publisher/PostLikePublisher.java, https://github.com/CorporationX/notification_service/blob/centaur-master-bc5/src/main/java/faang/school/notificationservice/listener/LikePostEventListener.java

## Implemented URL Shortener based on asynchronous cache to provide non-blocking handling of user requests.
link: https://github.com/grisatkac/url_shortener_service/blob/url-shortner-service-grisatkac/src/main/java/faang/school/urlshortenerservice/service/UrlService.java

## Implemented achievement feature
publisher: https://github.com/CorporationX/achievement_service/blob/feature-BJS2-25799/src/main/java/faang/school/achievement/publisher/AbstractMessagePublisher.java
consumer: https://github.com/CorporationX/achievement_service/blob/feature-BJS2-16049/src/main/java/faang/school/achievement/listener/PostEventListener.java

## Participated in News Feed implementation using publishing and consuming events by Kafka and Redis.
feed service: https://github.com/CorporationX/post_service/blob/feature-BJS2-27931/src/main/java/faang/school/postservice/service/feed/FeedService.java
publisher: https://github.com/CorporationX/post_service/blob/feature-BJS2-27931/src/main/java/faang/school/postservice/publisher/kafka/PostLikeKafkaPublisher.java 
consumer: https://github.com/CorporationX/post_service/blob/feature-BJS2-27931/src/main/java/faang/school/postservice/consumer/kafka/LikePostConsumer.java, 
cache: https://github.com/CorporationX/post_service/blob/feature-BJS2-27931/src/main/java/faang/school/postservice/cache/AbstractCache.java
