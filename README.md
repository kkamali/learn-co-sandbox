
Hi! 👋

You've opened the IDE Sandbox, an environment that you can access on "readme" and "code-along" lessons in Learn. It's a great place to experiment with code! 🎉

*IMPORTANT*
Saving varies by the type of work you are doing:
-- Most of the work you do in the Sandbox is automatically saved on your behalf to the `learn-co-sandbox` repository in your GitHub account. Please DO NOT touch this repository in GitHub. Doing so will affect your Sandbox experience, and potentially cause your work to fall out of sync.
-- *Git repositories that you clone into the Sandbox are NOT automatically saved.* In this case, you are responsible for committing and pushing your work to GitHub. 

To learn more about the Sandbox, please visit http://help.learn.co/technical-support/learn-ide-in-browser/ide-in-browser-sandbox

firstmost_name = bands.reduce(nil) do |memo, (key, value)|
  # On the first pass, we don't have a name, so just grab the first one.
  memo = value[0] if !memo
 
  # Sort that array of names
  sorted_names = value.sort
 
  # If string comparison says the sorted name of the array is earlier than
  # the memo, it becomes the new memo.
  memo = sorted_names[0] if sorted_names[0] <= memo
 
  # Return the memo as per reduce rules
  # (Try adding 'p' in front of memo to see how it changes as the enumerate the
  # pair of the hash!)
  p memo
end