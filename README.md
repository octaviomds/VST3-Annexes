VST 3 is a general rework of the long-serving VST plug-in interface. It is not compatible with the older VST versions, but it includes some new features and possibilities. We have redesigned the API to make it not only far easier and more reliable for developers to work with, but have also provided completely new possibilities for plug-ins. These include:

1. Improved Performance with the Silence Flag

Processing can optionally be applied to plug-ins only when audio signals are present on their respective inputs, so VST 3 plug-ins can apply their processing economically and only when it is needed.

2. Multiple Dynamic I/Os

VST 3 plug-ins are no longer limited to a fixed number of inputs and outputs, and their I/O configuration can dynamically adapt to the channel configuration. Side-chains are also very easily realizable. This includes the possibility to deactivate unused busses after loading and even reactivate those when needed. This cleans up the mixer and further helps to reduce CPU load.

3. Sample-accurate Automation

VST 3 also features vastly improved parameter automation with sample accuracy and support for ramped automation data, allowing completely accurate and rapid parameter automation changes.

4. Logical Parameter Organization

The VST 3 plug-in parameters are displayed in a tree structure. Parameters are grouped into sections which represent the structure of the plug-in. Plug-ins can communicate their internal structure for the purpose of overview, but also for some associated functionality (eg. program-lists).

5. Resizeable UI Editor

VST 3 defines a way to allow resizing of the plug-in editor by a user.

6. Mouse Over Support

The host could ask the plug-in which parameter is under the mouse.

7. Context Menu Support

VST 3 defines a way to allow the host to add its own entries in the plug-in context menu of a specific parameter.

8. Channel Context Information

A VST 3 plug-in could access some channel information where it is instantiated: name, color, ...

9. Note Expression

VST 3 defines with Note Expression a new way of event controller editing. The plug-in is able to break free from the limitations of MIDI controller events by providing access to new VST 3 controller events that circumvent the laws of MIDI and provide articulation information for each individual note (event) in a polyphonic arrangement according to its noteId.

10. 3D Support

VST 3 supports new speaker configurations like Ambisonic, Atmos, Auro 3D or 22.2.

11. Factory Concept

VST 3 plug-in library could export multiple plug-ins and in this way replaces the shell concept of VST 2 (kPlugCategShell).

12. Support Remote control Representation

VST 3 plug-in can deliver a specific parameter mapping for remote controls like Nuage.

13. Others

While designing VST 3, we performed a careful analysis of the existing functionality of VST and rewrote the interfaces from scratch. In doing so, we focused a lot on providing clear interfaces and their documentation in order to avoid usage errors from the deepest possible layer. Some more features implemented specifically for developers include:

More stable technical host/plug-in environment
Advanced technical definition of the standard
Modular approach
Separation of UI and processing
Advanced Preset System
Multiple plug-ins per Library
Test Host included
Automated Testing Environment
Validator (small command line Test Host) and plug-in examples code included
