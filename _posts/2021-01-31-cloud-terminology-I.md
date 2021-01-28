Let's learn about some cloud terms!

I've been hearing bunch of terms about cloud technologies lately, without actually getting my head around what they meant. Recently, I decided to study on that subject and I started to create this glossary of cloud terms, this way I could use them as references for my upcoming posts ans studies on cloud technologies.

With the first post of "Cloud Terminology" series we are going to look at a small, but commonly used subset of cloud terms:
* Public Cloud
* Private Cloud
* Virtual Private Cloud

# Public Cloud

A Public Cloud is set of resource that are provided to you and other customers by a vendor.

Public Cloud enables us to provision resources on demand according to our needs. There are many different vendors on the public cloud and depending on what you need as you build your software, they may offer you solutions on different abstraction levels.

As these solutions' levels goes **deeper**, it gives you **more control on the resource**, however, this also means **greater overhead** since you'll have more things to do for that resource to be working properly.

And one of the greatest benefits about public cloud is that you only pay for what you use. This gives you the ability to optimize your expenses.

Take a look at the below diagram to visualize solutions at different levels. Starting from bare-metal, where you got all the control but you have to do almost everything by yourself to get your software up and running, to serverless services where you only concentrate on writing your application code and networking, scaling and all others are handled for you.

{% include figure image_path="../assets/images/content/different_levels_of_abstraction.png" alt="Different levels of cloud service abstractions" caption="By Nate Schutta (Developer Advocate, Pivotal) at SpringOne Platform 2018" %}

# Private Cloud

Private Cloud is having public cloud environment on the infrastructure that is dedicated for you. This brings the disadvantage of being limited by your infrastructure's limits and the advantage of having no other neighbors to share your resources with.

# Virtual Private Cloud

A Virutal Private Cloud is where a public cloud's resources are divided into divisions ("private clouds") and each division is isolated from each other and then assigned to a different owner, making them feel like they have their own private cloud - but actually its only there virtually. Just like virtual machines, there are no actual separate machines but we get the feeling of having separate machines with the isolation. Virtual Private Clouds are a type of [Hybrid Clouds](https://www.redhat.com/en/topics/cloud-computing/what-is-hybrid-cloud).

{% include figure image_path="../assets/images/content/different_clouds.png" alt="Different Cloud Types Visualization" caption="Different Cloud Types Visualization" %}

# An Analogy

Imagine the public cloud as an internet cafe where they have these computers and they charge you for the time you use them. The owner of the internet cafe can be tought as the vendor (where in real life that can be Amazon, Google, Microsoft etc.). When you go and there and ask for a computer they start your session on one of the available computers in the public area with others, using the same underlying infrastructure. 

And then imagine there are private gaming rooms where they provide you a isolated internet connection from the ones in the public area and from the other private gaming rooms. These rooms can be tought as virtual private clouds. 

Now imagine this internet cafe vendor provides you the service to build one of these private gaming rooms to your house using your house's infrastructure but with their computers and all the software in it.

# References

* [https://azure.microsoft.com/en-us/overview/what-are-private-public-hybrid-clouds/](https://azure.microsoft.com/en-us/overview/what-are-private-public-hybrid-clouds/)
* [https://www.cloudflare.com/learning/cloud/what-is-a-public-cloud/](https://www.cloudflare.com/learning/cloud/what-is-a-public-cloud/)
* [https://www.cloudflare.com/learning/cloud/what-is-a-virtual-private-cloud/](https://www.cloudflare.com/learning/cloud/what-is-a-virtual-private-cloud/)
* [https://www.redhat.com/en/topics/cloud-computing/what-is-public-cloud](https://www.redhat.com/en/topics/cloud-computing/what-is-public-cloud)
* [https://www.redhat.com/en/topics/cloud-computing/public-cloud-vs-private-cloud-and-hybrid-cloud](https://www.redhat.com/en/topics/cloud-computing/public-cloud-vs-private-cloud-and-hybrid-cloud)
* [https://www.youtube.com/watch?v=8tOj4A7jgWg](https://www.youtube.com/watch?v=8tOj4A7jgWg)