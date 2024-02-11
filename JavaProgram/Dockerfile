from openjdk
RUN mkdir /java
ADD Trial.java /java
WORKDIR /java
RUN ["javac", "Trial.java"]
CMD ["java","Trial"]