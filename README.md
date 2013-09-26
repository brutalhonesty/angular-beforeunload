# angular-onbeforeunload
Confirm dialog pop up if they try and (or accidently click away from) the page.
<code>
angular.module('YOUR_APP', ['angular-onbeforeunload'])
  .controller('MainCtrl', ['onBeforeUnload', function(onBeforeUnload) {
    $scope.$on('$locationChangeStart', onBeforeUnload.init())
  }]);
</code>
