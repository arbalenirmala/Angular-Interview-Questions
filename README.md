# Angular-Interview-Questions

<table>
  <tr>
    <td>1.</td>
    <td> Explain ng-content vs ng-template vs ng-container.</td>
  </tr>
  <tr>
    <td>2.</td>
    <td>You are building an Angular application with a search feature that calls an API every time the user types something. The problem is that every keystroke triggers an API call, leading to performance issues. Your task is to implement debouncing to reduce the number of API calls by ensuring only one API call is triggered after the user stops typing for a predefined period.</td>
  </tr>
  <tr>
    <td>3.</td>
    <td>Explain Throttling and Debouncing techniques</td>
  </tr>
  <tr>
    <td>4.</td>
    <td>Explain flatmap, exahaustmap, map , mergemap, switchmap, mergemap</td>
  </tr>
  <tr>
    <td>5.</td>
    <td>Explain Subject in angular</td>
  </tr>
  <tr>
    <td>6.</td>
    <td>Explain state management in Angular</td>
  </tr>
  <tr>
    <td>7.</td>
    <td><b>Explain Change detection strategies in Angular</b> <br>
      Angular provides two strategies <br>
      1.Default - Trigger: Any change (event, async task, input, etc.) triggers change detection across the entire component tree.
                  Behavior: All components are checked from top to bottom.
                  Usage: This is Angular’s default behavior.<br>
        @Component({ <br>
              selector: 'app-example',<br>
              templateUrl: './example.component.html',<br>
              changeDetection: ChangeDetectionStrategy.Default<br>
          }) <br>
      2.OnPush - Trigger: Change detection runs only when:
            An @Input() reference changes
            An event inside the component fires
            Observable emits (manually triggered with async pipe)
            You manually call markForCheck() or detectChanges()
            Behavior: Improves performance by skipping unchanged components.
            Usage: Best for pure, stateless components or heavy UIs.<br>
            @Component({<br>
                selector: 'app-fast',<br>
                templateUrl: './fast.component.html',<br>
                changeDetection: ChangeDetectionStrategy.OnPush<br>
            })
    </td>
  </tr>
  <tr>
    <td>8. </td>
    <td>Traditional CMS vs Headless CMS <br> 
      Traditional CMSes couple back-end and front-end code together, whereas headless systems use a decoupled architecture to integrate with multiple front ends.
    Headless CMSs use APIs to deliver content, allowing developers to use various frontend technologies and display content on different platforms.</td>
  </tr>
  <tr>
    <td>9.</td>
    <td><b>what is markForCheck()? explain with example.</b><br>
      It's a method provided by Angular’s ChangeDetectorRef that tells Angular to check this component and its children on the next change detection cycle.<br>
      You need markForCheck() when:<br>
      You're using ChangeDetectionStrategy.OnPush<br>
      A change happens outside of Angular’s zone<br><br>
      Example: setTimeout, setInterval, manual service update, WebSocket, etc.<br>
      Angular didn’t detect the change automatically, and your view is stale<br><br>
      Purpose--&gt;	Manually request Angular to check for changes<br>
      Used--&gt; with	OnPush components<br>
    Triggers--&gt;	A recheck of the component and its children<br>
    When to use--&gt; When change happens outside Angular’s detection zone
    </td>
  </tr>
  <tr>
    <td>10.</td>
    <td>How to measure performance of javascript code?</td>
  </tr>
  <tr>
    <td>11.</td>
    <td>What is signal?</td>
  </tr>
   <tr>
    <td>12.</td>
    <td>What is standalone component?</td>
  </tr>
  <tr>
    <td>13.</td>
    <td>How to restrict routes? How to stop loading particular routes?</td>
  </tr>
  <tr>
    <td>14.</td>
    <td>Pure Pipe vs Impure Pipe <br>
      Pure pipes are executed only when a pure change is detected in the input value. A pure change means either the primitive input value has changed or the object reference has changed. 
Pure pipes are suitable for calculations or transformations that depend solely on input data and do not rely on external factors. Examples include formatting dates, currencies, or numbers. <br>

Impure pipes are executed on every Angular component change detection cycle, regardless of whether the input value has changed. 
Impure pipes are used when the pipe's behavior depends on external factors or when the input might change frequently due to user interactions or other dynamic events. 
<br>

    </td>
  </tr>
   <tr>
    <td>15.</td>
    <td>How to pass data with routes?</td>
  </tr>
</table>

