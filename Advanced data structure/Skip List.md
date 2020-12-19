# Skip List
Src: https://www.youtube.com/watch?v=UGaOXaXAM5M

> - Skip list allows **fast** search and insertion 
> > - Search: O(log(n))
> > - Insertion: O(log(n)) 

## Building a skip list:
> 1. We have a linked list containing n number in ascending order.
> > ![image](https://user-images.githubusercontent.com/64374947/102693510-d03ed780-4223-11eb-95d2-76ab5e952fa4.png)
> 2. Add sentinel node in the front
> > ![image](https://user-images.githubusercontent.com/64374947/102693589-64a93a00-4224-11eb-90df-9994f149c4e1.png)
> 3. Traverse on the node one by one and do random algorithm using flip a coin{T , H}
> > - if coin is a tail height is not grow otherwise height is grow 
> > > first iteration
> > > ![image](https://user-images.githubusercontent.com/64374947/102693827-067d5680-4226-11eb-9e54-c29739ff5ab1.png)
> > > second iteration
> > > ![image](https://user-images.githubusercontent.com/64374947/102693966-bf439580-4226-11eb-8d75-e27f3de2f6eb.png)
> > > third iteration
> > > ![image](https://user-images.githubusercontent.com/64374947/102693992-ee5a0700-4226-11eb-8f3d-9f2eccfc7468.png)

> > **The most reasonable number of layer is log(n)**

## Search

> 1. Key = 15
> > ![image](https://user-images.githubusercontent.com/64374947/102694214-4e04e200-4228-11eb-8db7-9c8029a27b41.png)
> 2. Key = 8
> > ![image](https://user-images.githubusercontent.com/64374947/102694288-b81d8700-4228-11eb-9bfc-cf11c3cd8b15.png)
> > ![image](https://user-images.githubusercontent.com/64374947/102694314-d8e5dc80-4228-11eb-8b75-f4f47beee29a.png)
> > ![image](https://user-images.githubusercontent.com/64374947/102694325-f6b34180-4228-11eb-97b8-695a0e21c57d.png)
> > ![image](https://user-images.githubusercontent.com/64374947/102694358-24988600-4229-11eb-8232-2752816b4938.png)
> > ![image](https://user-images.githubusercontent.com/64374947/102694370-3aa64680-4229-11eb-9c71-f10e388bf74a.png)
