# Exercise in integrals 
Integrals in computer science are similar but also different from the integral known from mathematics this exercise will shown you some of the similarities but also some of the differences.

initially you will have to watch the following video about [approximation of the Riemann integral, i.e. area under the curve](https://www.khanacademy.org/math/ap-calculus-ab/ab-integration-new/ab-6-2/v/simple-riemann-approximation-using-rectangles?fbclid=IwAR1KN1Rl5ohtuVJp1VPafI5uEI6R1U1gPOHKx4KcoIajiCoM9nFtCFhPusY). Don't fear the fancy word, the Riemann integral is simply the integral known from high school. If you are unfamiliar the integral from high school I recommend you stop here and reacquaint yourself with it, e.g. using [this video](https://www.youtube.com/watch?v=rfG8ce4nNh0). 

After you have watched the video read the following code and try to understand it.
```{r}
# make a grid form 0-1, with 0.01 between the each point
delta_x = 0.01
grid = seq(0, 1, by = delta_x) 

# make a normal distribution of the grid truncated at 0 and 1
dens = dnorm(grid, mean = 0.5, sd = 0.1)

sum(dens*delta_x)
```
Using this code you should now be able to solve the following exercises:

- [ ] plot the grid and the density
- [ ] Why is the normal distribution truncated at 0 and 1. How would you change it so that it is not?
- [ ] What does the values of the grid correspond to in the video?
- [ ] What does dens correspond in the video?
- [ ] What does the following do line do `dens[1]*delta_x` and what way is that similar to `dens * delta`?
- [ ] What does the last bit of code do? (`sum(dens*delta_x)`)
