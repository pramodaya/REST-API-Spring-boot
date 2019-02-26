# REST-API-Spring-boot
quick rest api with spring boot and start.spring.io

step 01
  download spring initializer from https://start.spring.io/
  dependancies: JPA, Rest Repositories, Rest Repositories HAL Browser, H2
  
step 02
  build it in eclipse with maven

step 03
  make Beer.java, DemoApplication.java, RestRepository.java 
  inside src->main->java->com.example.demo package

step 04
  make DemoApplicationTests.java 
  inside src->java->com.example.demo package

step 05
  make application.properties, data.sql 
  inside src->main->resources 

step 06
   run and go to http://localhost:8080/beers 


output: 

{
  "_embedded" : {
    "beers" : [ {
      "name" : "jai",
      "abv" : 2.3,
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/beers/1"
        },
        "beer" : {
          "href" : "http://localhost:8080/beers/1"
        }
      }
    }, {
      "name" : "stone",
      "abv" : 4.3,
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/beers/2"
        },
        "beer" : {
          "href" : "http://localhost:8080/beers/2"
        }
      }
    }, {
      "name" : "rock",
      "abv" : 6.3,
      "_links" : {
        "self" : {
          "href" : "http://localhost:8080/beers/3"
        },
        "beer" : {
          "href" : "http://localhost:8080/beers/3"
        }
      }
    } ]
  },
  "_links" : {
    "self" : {
      "href" : "http://localhost:8080/beers"
    },
    "profile" : {
      "href" : "http://localhost:8080/profile/beers"
    }
  }
}
