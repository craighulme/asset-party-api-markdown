# Panel

## 
```c#
Implements IPanel
```

## Summary

A simple User Interface panel. Can be styled withCSS.Ultimately must be a child of aUI.RootPanel.
This can be a customHudEntity<RootPanel>that is spawned by yourGameManager, aWorldPanel, or a rawUI.RootPanel.
## Constructors

```c#
Panel( ) 
```
No Summary
```c#
Panel( Panel parent) 
```
No Summary
```c#
Panel( Panel parent, string classnames) 
```
No Summary
## Fields

```c#
protected List<Panel> _children
```
List of panels that are attached/parenteddirectly to this one.
```c#
protected HashSet<Panel> _childrenHash
```
Used internally.
PAINDAY TODO: internalize
```c#
protected HashSet<string> _class
```
A list of CSS classes applied to this panel.
```c#
protected Panel _parent
```
The panel we are directly attached to. This panel will be positioned relative to the given parent, and therefore move with it, typically also be hidden by the parents bounds.
```c#
Vector2 ScrollVelocity
```
The velocity of the current scroll
```c#
StyleSheetCollection StyleSheet
```
A collection of stylesheets applied to this panel directly.
```c#
TaskSource Task
```
Quick access to timing events, for async/await.
## Properties

```c#
virtual bool AcceptsImeInput { get; } 
```
False by default. Anything that is capable of accepting IME input should return true. Which is probably just a TextEntry.
```c#
virtual IEnumerable<IStyleBlock> ActiveStyleBlocks { get; } 
```
ImplementsIPanel.ActiveStyleBlocksA importance sorted list of style blocks that are active on this panel
```c#
virtual PanelInputType ButtonInput { get; set; } 
```
ImplementsIPanel.ButtonInputDescribe what to do with keyboard input. The default is InputMode.UI which means that when
focused, this panel will receive Keys Typed and Button Events.
If you set this to InputMode.Game, this panel will redirect its inputs to the game, which means
for example that if you're focused on this panel and press space, it'll send the jump button to the game.
```c#
virtual bool HasContent { get; } 
```
If true, callsPanel.DrawContent.
```c#
virtual bool HasTooltip { get; } 
```
ImplementsIPanel.HasTooltipYou should override and return true if you're overridingPanel.CreateTooltipPanel.
Otherwise this will return true ifPanel.Tooltipis not empty.
```c#
virtual string Id { get; set; } 
```
ImplementsIPanel.IdWorks the same as the html id="" attribute. If you set Id to "poop", it'll match any styles
that define #poop in their selector.
```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidWhether this object is valid or not.
```c#
virtual PseudoClass PseudoClass { get; set; } 
```
ImplementsIPanel.PseudoClassSpecial flags used by the styling system for hover, active etc..
```c#
virtual string SourceFile { get; set; } 
```
ImplementsIPanel.SourceFileIf this was created by razor, this is the file in which it was created
```c#
virtual int SourceLine { get; set; } 
```
ImplementsIPanel.SourceLineIf this was created by razor, this is the line number in the file
```c#
virtual string StringValue { get; set; } 
```
Set via"value"property from HTML.
```c#
virtual bool WantsDrag { get; } 
```
Return true if this panel wants to be dragged
```c#
protected virtual bool WantsDragScrolling { get; } 
```
No Summary
```c#
bool AcceptsFocus { get; set; } 
```
False by default, can this element accept keyboard focus. If an element accepts
focus it'll be able to receive keyboard input.
```c#
PanelCreator Add { get; } 
```
Quickly add common panels with certain values as children.
```c#
bool AllowChildSelection { get; set; } 
```
Allow selecting child text
```c#
IEnumerable<StyleSheet> AllStyleSheets { get; } 
```
List of allUI.StyleSheets applied to this panel and all itsancestors.
```c#
IEnumerable<Panel> Ancestors { get; } 
```
Returns all ancestors, i.e. the parent, parent of our parent, etc.
```c#
IEnumerable<Panel> AncestorsAndSelf { get; } 
```
Returns this panel and all itsancestors, i.e. theParent, parent of its parent, etc.
```c#
Box Box { get; init; } 
```
Access to various bounding boxes of this panel.
```c#
bool CanDragScroll { get; set; } 
```
Set this to false if you want to opt out of drag scrolling
```c#
RenderFragment ChildContent { get; set; } 
```
No Summary
```c#
IEnumerable<Panel> Children { get; } 
```
ImplementsIPanel.ChildrenList of panels that are attached/parenteddirectly to this one.
```c#
int ChildrenCount { get; } 
```
ImplementsIPanel.ChildrenCountAmount of panels directlyparentedto this panel.
```c#
IEnumerable<string> Class { get; } 
```
A list of CSS classes applied to this panel.
```c#
string Classes { get; set; } 
```
ImplementsIPanel.ClassesAll CSS classes applied to this panel, separated with spaces.
```c#
Styles ComputedStyle { get; } 
```
This is the style that we computed last. If you're looking to see which
styles are set on this panel then this is what you're looking for.
```c#
CancellationToken DeletionToken { get; } 
```
Get a token that is cancelled when the panel is deleted
```c#
IEnumerable<Panel> Descendants { get; } 
```
List of all panels that are attached to this panel, recursively, i.e. allchildrenof this panel, children of those children, etc.
```c#
string ElementName { get; set; } 
```
ImplementsIPanel.ElementNameThe element name. If you've created this Panel via a template this will be whatever the element
name is on there. If not then it'll be the name of the class (ie Panel, Button)
```c#
Matrix? GlobalMatrix { get; } 
```
ImplementsIPanel.GlobalMatrixIf this panel or its parents have transforms, they'll be compounded here.
```c#
bool HasActive { get; } 
```
Whether this panel has the:activepseudo class active.
```c#
bool HasActiveTransitions { get; } 
```
Returns true if this panel has any active CSS transitions.
```c#
bool HasChildren { get; } 
```
Whether this panel has anychild panelsat all.
```c#
bool HasFocus { get; } 
```
Whether this panel has the:focuspseudo class active.
```c#
bool HasHovered { get; } 
```
Whether this panel has the:hoverpseudo class active.
```c#
bool HasIntro { get; } 
```
Whether this panel has the:intropseudo class active.
```c#
bool HasMouseCapture { get; } 
```
Whether this panel is capturing the mouse cursor. SeePanel.SetMouseCapture.
```c#
bool HasOutro { get; } 
```
Whether this panel has the:outropseudo class active.
```c#
bool HasScrollX { get; } 
```
Return true if this panel is scrollable on the X axis
```c#
bool HasScrollY { get; } 
```
Return true if this panel is scrollable on the Y axis
```c#
bool IsDeleting { get; } 
```
WhetherPanel.Deletewas called on this panel.
```c#
bool IsScrollAtBottom { get; } 
```
Whether the scrolling is currently pinned to the bottom of the panel as dictated byPanel.PreferScrollToBottom.
```c#
bool IsVisible { get; } 
```
ImplementsIPanel.IsVisibleReturn true if this panel isn't hidden by opacity or displaymode.
```c#
bool IsVisibleSelf { get; } 
```
ImplementsIPanel.IsVisibleSelfReturn true if this panel isn't hidden by opacity or displaymode.
```c#
Matrix? LocalMatrix { get; } 
```
If this panel has transforms, they'll be reflected here
```c#
Vector2 MousePosition { get; } 
```
Current mouse position local to this panels top left corner.
```c#
float Now { get; } 
```
No Summary
```c#
float Opacity { get; } 
```
The currently calculated opacity.
This is set by multiplying our current style opacity with our parent's opacity.
```c#
Panel Parent { get; set; } 
```
ImplementsIPanel.ParentThe panel we are directly attached to. This panel will be positioned relative to the given parent, and therefore move with it, typically also be hidden by the parents bounds.
```c#
bool PreferScrollToBottom { get; set; } 
```
If true, we'll try to stay scrolled to the bottom when the panel changes size
```c#
float ScaleFromScreen { get; } 
```
Inverse scale ofPanel.ScaleToScreen.
```c#
float ScaleToScreen { get; } 
```
Scale of the panel on the screen.
```c#
Vector2 ScrollOffset { get; set; } 
```
Offset of the panel's children position for scrolling purposes.
```c#
Vector2 ScrollSize { get; } 
```
The size of the scrollable area within this panel.
```c#
int SiblingIndex { get; } 
```
The index of this panel in its parent's child list.
```c#
PanelStyle Style { get; } 
```
Allows you to set styles specifically on this panel. Setting the style will
only affect this panel and no others and will override any other styles.
```c#
string Tooltip { get; set; } 
```
A string to show when hovering over this panel.
```c#
Transitions Transitions { get; } 
```
Handles the storage, progression and application of CSS transitions.
```c#
object UserData { get; set; } 
```
Can be used to store random data without sub-classing the panel.
## Methods

```c#
protected virtual void AddScrollVelocity( ) 
```
No Summary
```c#
protected virtual int BuildHash( ) 
```
By overriding this you can return a hash of variables used by the Razor layout, which
will cause a rebuild when changed. This is useful when your layout uses a global variable
because by adding it to a HashCode.Combine here you can easily trigger a build when it changes.
```c#
protected virtual void BuildRenderTree( RenderTreeBuilder tree) 
```
Overridden/implemented by Razor templating to build a render tree.
```c#
protected virtual void ConstrainScrolling( Vector2 size) 
```
Constrainscrollingto the given size.
```c#
virtual void CreateEvent( string name, object value = null, float? debounce = null) 
```
Create a new event and pass it to the panels event queue.
```c#
virtual void CreateEvent( PanelEvent evnt) 
```
Pass given event to the event queue.
```c#
protected virtual Panel CreateTooltipPanel( ) 
```
Create a tooltip panel. You can override this to create a custom tooltip panel.If you're overriding this and not settingPanel.Tooltip, then you must override and return true inPanel.HasTooltip.
```c#
virtual void Delete( bool immediate = false) 
```
ImplementsIPanel.DeleteDeletes the panel.
```c#
virtual void DrawBackground( ref RenderState state) 
```
Called to draw the panels background.
```c#
virtual void DrawContent( ref RenderState state) 
```
Called whenPanel.HasContentis set totrueto custom draw the panels content.
```c#
virtual void FinalLayout( Vector2 offset) 
```
Takes aUI.LayoutCascadeand returns an outer rect
```c#
protected virtual void FinalLayoutChildren( Vector2 offset) 
```
Layout the children of this panel.
```c#
virtual Panel FindPopupPanel( ) 
```
Returns the firstancestorpanel that has no parent.
```c#
virtual string GetClipboardValue( bool cut) 
```
If we have a value that can be copied to the clipboard, return it here.
```c#
protected virtual string GetRenderTreeChecksum( ) 
```
Overridden/implemented by Razor templating, contains render tree checksum to determine when the render tree content has changed.
```c#
virtual Vector2 GetTransformPosition( Vector2 pos) 
```
Called by Sandbox.UI.PanelInput.CheckHover(Sandbox.UI.Panel,Vector2,Sandbox.UI.Panel@) to transform
the current mouse position using the panel's LocalMatrix (by default). This can be overriden for special cases.
```c#
protected virtual void InitializeEvents( ) 
```
Called on creation and hotload to delete and re-initialize event listeners.
```c#
virtual void LanguageChanged( ) 
```
Called when the current language has changed. This allows you to rebuild
anything that might need rebuilding. Tokenized text labels should automatically update.
```c#
protected virtual void OnAfterTreeRender( bool firstTime) 
```
Called after the razor tree has been created/rendered.
```c#
protected virtual void OnBack( PanelEvent e) 
```
Called when the player presses the "Back" button while hovering this panel, which is typically "mouse 5", aka one of the mouse buttons on its side.
```c#
protected virtual void OnBlur( PanelEvent e) 
```
Called when this panel loses input focus.
```c#
virtual void OnButtonEvent( ButtonEvent e) 
```
Called when any button, mouse (except for mouse4/5) and keyboard, are pressed or depressed while hovering this panel.
```c#
virtual void OnButtonTyped( ButtonEvent e) 
```
Called when any keyboard button has been typed (pressed) while this panel has input focus. (Panel.Focus)
```c#
virtual void OnButtonTyped( string button, KeyModifiers km) 
```
No Summary
```c#
protected virtual void OnChildAdded( Panel child) 
```
A child panel has been added to this panel.
```c#
protected virtual void OnChildRemoved( Panel child) 
```
A child panel has been removed from this panel.
```c#
protected virtual void OnClick( MousePanelEvent e) 
```
Called when the player releases their left mouse button (Mouse 1) while hovering this panel.
```c#
virtual void OnDeleted( ) 
```
Called when the panel is about to be deleted.
```c#
protected virtual void OnDoubleClick( MousePanelEvent e) 
```
Called when the player double clicks the panel with the left mouse button.
```c#
protected virtual void OnDrag( DragEvent e) 
```
No Summary
```c#
protected virtual void OnDragEnd( DragEvent e) 
```
No Summary
```c#
protected virtual void OnDragSelect( SelectionEvent e) 
```
Called when the player moves the mouse after "press and holding" (or dragging) the panel.
```c#
protected virtual void OnDragStart( DragEvent e) 
```
No Summary
```c#
protected virtual void OnEscape( PanelEvent e) 
```
Called when the escape key is pressed
```c#
protected virtual void OnEvent( PanelEvent e) 
```
Called when variousUI.PanelEvents happen. Handles event listeners and many standard events by default.
```c#
protected virtual void OnFocus( PanelEvent e) 
```
Called when this panel receives input focus.
```c#
protected virtual void OnForward( PanelEvent e) 
```
Called when the player presses the "Forward" button while hovering this panel, which is typically "mouse 4", aka one of the mouse buttons on its side.
```c#
virtual void OnHotloaded( ) 
```
Called when a hotload happened. (Not necessarily on this panel)
```c#
virtual void OnKeyTyped( Char k) 
```
Called when a printable character has been typed (pressed) while this panel has input focus. (Panel.Focus)
```c#
virtual void OnLayout( ref Rect layoutRect) 
```
This panel has just been laid out. You can modify its position now and it will affect its children.
This is a useful place to restrict shit to the screen etc.
```c#
protected virtual void OnMiddleClick( MousePanelEvent e) 
```
Called when the player releases their middle mouse button (Mouse 3) while hovering this panel.
```c#
protected virtual void OnMouseDown( MousePanelEvent e) 
```
Called when the player presses down the left or right mouse buttons while hovering this panel.
```c#
protected virtual void OnMouseMove( MousePanelEvent e) 
```
Called when the cursor moves while hovering this panel.
```c#
protected virtual void OnMouseOut( MousePanelEvent e) 
```
Called when the cursor leaves this panel.
```c#
protected virtual void OnMouseOver( MousePanelEvent e) 
```
Called when the cursor enters this panel.
```c#
protected virtual void OnMouseUp( MousePanelEvent e) 
```
Called when the player releases left or right mouse button.
```c#
virtual void OnMouseWheel( float value) 
```
Called when the player scrolls their mouse wheel while hovering this panel.
```c#
protected virtual void OnParametersSet( ) 
```
Called after all templated panel binds have been set.
```c#
protected virtual Task OnParametersSetAsync( ) 
```
Called after all templated panel binds have been set.
```c#
virtual void OnParentChanged( ) 
```
Called after the parent of this panel has changed.
```c#
virtual void OnPaste( string text) 
```
Called when the user presses CTRL+V while this panel has input focus.
```c#
protected virtual void OnRightClick( MousePanelEvent e) 
```
Called when the player releases their right mouse button (Mouse 2) while hovering this panel.
```c#
virtual bool OnTemplateElement( INode element) 
```
No Summary
```c#
virtual void OnTemplateSlot( INode element, string slotName, Panel panel) 
```
TODO: Obsolete this and instead maybe we have something like [PanelSlot( "slotname" )] that
is applied on properties. Then when we find a slot="slotname" we chase up the heirachy and set the property.
```c#
virtual bool RayToLocalPosition( Ray ray, out Vector2 position, out float distance) 
```
Transform a ray in 3D space to a position on the panel. This is used for world panel input.
```c#
virtual void SetContent( string value) 
```
Called by the templating system when an element has content between its tags.
```c#
virtual void SetProperty( string name, string value) 
```
Set a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
```c#
virtual void SetPropertyObject( string name, object value) 
```
Same asPanel.SetProperty, but first tries to set the property on the panel object, then process any special properties such asclass.
```c#
virtual void Tick( ) 
```
Called every frame. This is your "Think" function.
```c#
virtual bool WantsMouseInput( ) 
```
Returns true if this panel would like the mouse cursor to be visible.
```c#
void AddChild( Panel p) 
```
Add given panel as a child to this panel.
```c#
T AddChild<T,>( string classnames = null) 
```
Creates a panel of given type and makes it our child.
```c#
bool AddChild<T,>( out T outPanel, string classnames = null) 
```
Creates a panel of given type and makes it our child, returning it as an out argument.
```c#
void AddClass( string classname) 
```
Adds CSS class(es) separated by spaces to this panel.
```c#
void AddEventListener( string eventName, Action<PanelEvent> e) 
```
Runs given callback when the given event is triggered.
```c#
void AddEventListener( string eventName, Action action) 
```
Runs given callback when the given event is triggered, without access to theUI.PanelEvent.
```c#
void Bind( string ourPropertyName, object targetObject, string theirPropertyName) 
```
No Summary
```c#
void BindClass( string className, Func<bool> func) 
```
Switch the class on or off depending on the value of the bool.
```c#
bool Blur( ) 
```
Remove input focus from this panel.
```c#
IEnumerable<T> ChildrenOfType<T,>( ) 
```
Returns a list ofchild panelsof given type.
```c#
protected void CreateValueEvent( string name, object value) 
```
Call this when the value has changed due to user input etc. This updates any
bindings, backwards. Also triggers $".changed" event, with value being the Value on the event.
```c#
void DeleteChildren( bool immediate = false) 
```
Deletes all child panels viaPanel.Delete.
```c#
IEnumerable<Panel> FindInRect( Rect box, bool fullyInside) 
```
Find and return any children of this panel (including self) within the given rect.
```c#
RootPanel FindRootPanel( ) 
```
Returns theUI.RootPanelwe are ultimately attached to, if any.
```c#
bool Focus( ) 
```
Give input focus to this panel.
```c#
string GetAttribute( string k, string defaultIfNotFound = null) 
```
Used in templates, try to get the attribute that was set in creation.
```c#
Panel GetChild( int index, bool loop = false) 
```
Return a child at given index.
```c#
int GetChildIndex( Panel panel) 
```
Returns the index at which the given panel isparentedto this panel, or -1 if it is not.
```c#
bool HasClass( string classname) 
```
Whether we have the given CSS class or not.
```c#
bool IsAncestor( Panel panel) 
```
ImplementsIPanel.IsAncestorIs the given panel a parent, grandparent, etc.
```c#
bool IsInside( Vector2 pos) 
```
Whether given screen position is within this panel. This will accurately handle border radius as well.
```c#
bool IsInside( Rect rect, bool fullyInside) 
```
Whether the given rect is inside this panels bounds. (Box.Rect)
```c#
void MoveAfterSibling( Panel previousSibling) 
```
Move this panel to be after the given sibling.
```c#
Vector2 PanelPositionToScreenPosition( Vector2 pos) 
```
Convert a point from local space to screen space
```c#
void PlaySound( string sound) 
```
Play a sound from this panel.
```c#
void RemoveClass( string classname) 
```
Removes given CSS class from this panel.
```c#
Vector2 ScreenPositionToPanelDelta( Vector2 pos) 
```
Convert a point from the screen to a point representing a delta on this panel where
the top left is [0,0] and the bottom right is [1,1]
```c#
Vector2 ScreenPositionToPanelPosition( Vector2 pos) 
```
Convert a point from the screen to a position relative to the top left of this panel
```c#
void SetAttribute( string k, string v) 
```
Used in templates, gets an attribute that was set in the template.
```c#
void SetChildIndex( Panel child, int newIndex) 
```
Move given child panel to be given index, where 0 is the first child.
```c#
void SetClass( string classname, bool active) 
```
Sets a specific CSS class active or not.
```c#
void SetMouseCapture( bool b) 
```
Captures the mouse cursor while active. The cursor will be hidden and will be stuck in place.You will want to useMouse.DeltainPanel.TickwhilePanel.HasMouseCaptureto read mouse movements.You can call this fromPanel.OnButtonEventfor mouse clicks.
```c#
void SetTemplate( string filename) 
```
No Summary
```c#
void SkipTransitions( ) 
```
Any transitions running, or about to run, will jump straight to the end.
```c#
void SortChildren( Comparison<Panel> sorter) 
```
Sort thechildrenusing given comparison function.
```c#
void SortChildren<TargetType,>( Func<TargetType, int> sorter) 
```
Sort thechildrenusing given comparison function.
```c#
void SortChildren( Func<Panel, int> sorter) 
```
Sort thechildrenusing given comparison function.
```c#
void StateHasChanged( ) 
```
For razor panels, call when the state of the render tree has changed such that
it would be a good idea to re-render the tree. You would usually not need to call
this manually.
```c#
protected void StyleSelectorsChanged( bool ancestors, bool descendants, RootPanel root = null) 
```
Should be called when something happens that means that this panel's stylesheets need to be
re-evaluated. Like becoming hovered or classes changed. You don't call this when changing styles
directly on the panel, just on anything that will change which stylesheets should get selected.
```c#
bool Switch( PseudoClass c, bool state) 
```
Switch a pseudo class on or off.
```c#
bool TryFindKeyframe( string name, out KeyFrames keyframes) 
```
Try to find@keyframesCSS rule with given name inPanel.AllStyleSheets.
```c#
bool TryScroll( float value) 
```
Called fromPanel.OnMouseWheelto try to scroll.
```c#
bool TryScrollToBottom( ) 
```
Scroll to the bottom, if the panel has scrolling enabled.
## Extensions

```c#
void Navigate( string url) 
```
Find the closest navigatorPanel ancestor and navigate to the given url
## Inheriting Types

