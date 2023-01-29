# CohesionAndCoupling
Cohesion And Coupling With .Net





# Intended Audience
1+ yrs of development experience

# Definition
Cohesion is defined as the degree of relationship between elements of the same module. Coupling is defined as the degree of interdependence between the modules.

Coupling is all about how classes interact with each other, on the other hand cohesion focuses on how single class is designed

High coupling and loose coupling should be followed everywhere as per best practices under OOPS principles.

# Reason for Writing
I couldnt find crystal clear understanding of cohesion and coupling over the internet.

# Real use case High Cohesion
We want to write functionality for user registration and we need to check if the user age is greater than 18
to allow for registration. 

public class User
    {
        private string fullName;
        private int age;

        public string FullName { get;  }
        public int Age { get; }

        public bool CanUserRegister()
        {
            if (this.age >= 18)
                return true;

            return false;
        }
    }

In this example CanUserRegister() method is written inside User class and not in any other file/place. This is 
an example of high cohesion as the related relationship is kept in same class

Real use case Loose Coupling Coupling-
https://github.com/tarunprof4/NLayerArchitecture-LooselyCoupled/blob/main/README.md
