# Admin-cheat-sheet

```
rails g migration add_superadmin_logic_to_users
```
```
add_column :users, :is_superadmin,:boolean, default: false
```


 ``` namespace :superadmin do
    root :to => 'admin#index'
    resources :picture, except: [:new, :create]
    resources :users, except: [:new , :create]
  end
  ```
  ```
  rails g controller superadmin/picture index show new create update destroy
  rails g controller superadmin/users index show new create update destroy
  ```
  

### rendre un user SuperAdmin

#### apres
```
voir mon repo event triple originale
```
