PopupView=======![sample image](http://sonson.jp/wp/wp-content/uploads/2011/07/popupViewSample1.png)License=======BSD License.SNPopupView Reference=======	- (id)initWithString:(NSString*)newValue;###Parameters####newValueThre string to display as title in the popup.###Return valueAn initialized popup.###DiscussionThis method uses default title's font size. If you want to set own font size for title, you should use initWithString:withFontOfSize:.	- (id)initWithString:(NSString*)newValue withFontOfSize:(float)newFontSize;###Parameters####newValueThre string to display as title in the popup.####newFontSizeThe point size of the font for title.###Return valueAn initialized popup.###DiscussionThis method does not automatically adjust font size of title. Therefore, the title string can go over popup view if you specfy too big font size.		- (id)initWithImage:(UIImage*)newImage;###Parameters####newImageThe image to display in the popup.###Return valueAn initialized popup.###DiscussionNone.	- (id)initWithContentView:(UIView*)newContentView contentSize:(CGSize)contentSize;###Parameters####newContentViewThe new view whose content should be displayed by popup.####contentSizeThe new size to apply to the content view.###Return valueAn initialized popup.###DiscussionNone.	- (void)showAtPoint:(CGPoint)p inView:(UIView*)inView;###Parameters####pThe position to display popup withing the coordinate system of popup's superview, that is inView. Popup anchors at this point.####inViewThe view to set as popup' superview.###DiscussionNone.	- (void)showAtPoint:(CGPoint)p inView:(UIView*)inView animated:(BOOL)animated;###Parameters####pThe position to display popup withing the coordinate system of popup's superview, that is inView. Popup anchors at this point.####inViewThe view to contain popup.####animatedSpecify YES to show it with animation, NO to show it immediately.###DiscussionNone.	- (void)showFromBarButtonItem:(UIBarButtonItem*)barButtonItem inView:(UIView*)inView;###Parameters####barButtonItemThe bar button item on which to anchor the popup.####inViewThe view to contain popup.###DiscussionNone.	- (void)showFromBarButtonItem:(UIBarButtonItem*)barButtonItem inView:(UIView*)inView animated:(BOOL)animated;###Parameters####barButtonItemThe bar button item on which to anchor the popup.####inViewThe view to contain popup.####animatedSpecify YES to show it with animation, NO to show it immediately.###DiscussionNone.		- (void)dismiss;###DiscussionDismiss popup with animation.	- (void)dismiss:(BOOL)animtaed;###Parameters####animatedSpecify YES to dimiss it with animation, NO to dimiss it immediately.###DiscussionNone.	- (void)addTarget:(id)target action:(SEL)action;###Prameters####targetThe target object-that is, the object to which the action message is sent. If this is nil, the responder chain is searched for an object willing to respond to the action message.####actionA selector identifying an action message. It cannot be NULL.###DiscussionProperties======###titleThe receiver's title string value.@property(nonatomic, readonly) NSString *title;###Discussion###imageThe receiver's image value.@property(nonatomic, readonly) UIImage *image;###DiscussionBlog======= * [sonson.jp][]Sorry, Japanese only....Dependency======= * none[sonson.jp]: http://sonson.jp