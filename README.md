# MRTKExamples
Place to dump prototype MRTK examples for Slack and other MRTK people!
This is just a GitHub dump for misc UnityPackages associated with MRTK V2 RC1.

#Unity Project Setup
Make sure you already have a Unity Project with MRTK in it. This package was created in Unity 2019.1.3f1.
Package contains a modified Unity Scene from the original MRTK V2 RC1 - hence the MRTK requirement :) 
Import the package.

#Testing the Runtime Interactable Modifications
If there were no issues on the package import, Look for the Directory '{Your Unity Project Folder}'/Assets/JFuzzMRTK/RunTime/Scenes/HandInteractionExampleModified.scene

1. Find the Pine tree and look at the GameObject called 'node_id30' it has two added scripts from this package, 'RunTimeBaseTester.cs' & 'RunTimeBaseAdjust.cs'
2. At runtime hit the 'O' key to add an OnFocus runtime method called 'DynamicFunctionOne'
Focus on the tree - notice the Debug Statement when you OnFocus with a controller/raycast
3. Now, in the editor change the 'MethodName' to 'DynamicFunctionTwo' and in the play screen hit the 'X' key adding another method, Focus on the object and focus off - you should see that the off focus is now also displaying a secondary debug log out.

For a better explaination see the video here: [YouTube Reference Video](https://youtu.be/47OExTOOuyU)
