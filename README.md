# DnSpyNoComments
So let's imagine this, you're trying to decompile an app with DnSpy, and you're most likely exporting to solution.
You would like to show it to people, but it's a relatively huge project, so you are annoyed by the huge quantity of the (maybe useless to you) comments.

# What I've done
In the code of DnSpy there's this method:
```cs
void AddComment(AstNode node, IMemberDef member, string text = null)
		{
    ...
    }
```
Since I didn't want to be bothered to setup the DnSpy project, I funnily decided to use DnSpy to fix up the DnSpy problem 😆.
I used IL editing to change it from the beforementioned code to 
```cs
void AddComment(AstNode node, IMemberDef member, string text = null)
		{
    }
```

# How do I download the fix? 
All you need to do is download the binary from the master branch then put it inside DnSpy\bin and replace.
