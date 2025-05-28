# Angular-Interview-Questions

<table>
  <tr>
    <td>1.</td>
    <td> Explain ng-content vs ng-templte vs ng-container.</td>
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
    <td>Explain Change detection strategies in Angular <br>
      Angular provides two strategies 
      1.Default - Trigger: Any change (event, async task, input, etc.) triggers change detection across the entire component tree.
                  Behavior: All components are checked from top to bottom.
                  Usage: This is Angular’s default behavior.<br>
        @Component({
              selector: 'app-example',
              templateUrl: './example.component.html',
              changeDetection: ChangeDetectionStrategy.Default
          })
      2.OnPush - Trigger: Change detection runs only when:
            An @Input() reference changes
            An event inside the component fires
            Observable emits (manually triggered with async pipe)
            You manually call markForCheck() or detectChanges()
            Behavior: Improves performance by skipping unchanged components.
            Usage: Best for pure, stateless components or heavy UIs.<br>
            @Component({
                selector: 'app-fast',
                templateUrl: './fast.component.html',
                changeDetection: ChangeDetectionStrategy.OnPush
            })
    </td>
  </tr>
  <tr>
    <td>8. </td>
    <td>Traditional CMS vs Headless CMS <br> 
      Traditional CMSes couple back-end and front-end code together, whereas headless systems use a decoupled architecture to integrate with multiple front ends.
    Headless CMSs use APIs to deliver content, allowing developers to use various frontend technologies and display content on different platforms.</td>
  </tr>
</table>

