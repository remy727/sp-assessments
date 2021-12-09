## Ruby on Rails

#### Q1. What is the **class** of `true`?
- [ ] `Boolean`
- [ ] `True`
- [ ] `TrueClass`

#### Q2. Which one validates the record?
- [ ] `update_attributes`
- [ ] `update_attribute`
- [ ] `update_column`

#### Q3 Within a Rails controller, which code will prevent the parent controller's before_action `:check_permission` from running?
- [ ] `skip_before_action :check_permission`
- [ ] `skip :check_permission, except: []`
- [ ] `prevent_action :check_permission`
- [ ] `:redis_cache_store`

#### Q4. When using an ActiveRecord model, which method will create the model instance in memory and save it to the database?
- [ ] `build`
- [ ] `new`
- [ ] `create`
- [ ] `save`

#### Q5. Which module can you use to encapsulate a cohesive chunk of functionality into a mixin?
- [ ] `ActiveSupport::Concern`
- [ ] `RailsHelper.CommonClass`
- [ ] `ActiveJob::Mixin`
- [ ] `ActiveSupport::Module`

#### Q6. Where should you put images, JavaScript, and CSS so that they get processed by the asset pipeline?
- [ ] app/static
- [ ] app/images
- [ ] app/assets
- [ ] app/views

#### Q7. Which one is not Design Pattern?
- [ ] Service
- [ ] Lib
- [ ] Decorator
- [ ] Factory

#### Q8. If a product has a user-uploadable photo, which ActiveStorage method should fill in the blank?

```
class Product << ApplicationRecord
  ____ :photo
end

```

- [ ] has_one_attached
- [ ] has_image
- [ ] attached_file
- [ ] acts_as_attachment

#### Q9. Given a table of blog_posts and a related table of comments (comments made on each blog post), which ActiveRecord query will retrieve all blog posts with comments created during @range?

- [ ] BlogPost.joins (:comments).where(comments: {created_at: @range})
- [ ] BlogPost.where(['comments.created_at', @range])
- [ ] BlogPost.preload ("comments.created_at").where(created_at: @range)
- [ ] BlogPost.includes (:comments).where('comments.created_at' => @range)

#### Q10. After this migration has been executed, which statement would be true?

```ruby
class CreateProducts < ActiveRecord::Migration
  def change
    create_table :products do |t|
      t.string :name, :bg_color
      t.integer :position
      t.boolean :visible, default: false
      t.timestamps
    end
  end
end
```

- [ ] The products table will have no primary key.
- [ ] The products table will include a column named "updated_at".
- [ ] The products table will contain exactly seven columns.
- [ ] The products table will have an index on the position column.