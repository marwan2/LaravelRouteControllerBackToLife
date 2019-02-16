# LaravelRouteControllerBackToLife
Return Laravel Route::controller back to the framework for Laravel 5.5 and above

Simply replace The Laravel main Router class "vendor/laravel/framework/src/Illuminate/Routing/Router.php" with this one.

And enjoy using Route::controller that you love, and your old projects use it too much.

Please note that any update from Laravel itsself, may overwrite this file, so you may need to add only the following methods from this Class to Router.php class
- public function controller($uri, $controller, $names = [])
- protected function prependGroupUses($uses)
- protected function registerInspected($route, $controller, $method, &$names)
- protected function addFallthroughRoute($controller, $uri)
