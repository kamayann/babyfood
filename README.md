## usersテーブル

| Column             | Type        | Options                   |
| ------------------ | ----------- | ------------------------- |
| email              | string      | null: false, unique: true |
| encrypted_password | string      | null: false               |
| nickname           | string      | null: false               |
| relationship       | integer     | null: false               |

### Association
- has_many :babys

## babysテーブル

| Column              | Type       | Options                        |
| ------------------- | ---------- | ------------------------------ |
| nickname            | string     | null: false                    |
| age                 | integer    | null: false                    |

### Association
- belongs_to :user
- has_many :meals


## mealsテーブル

| Column             | Type       | Options                        |
| ------------------ | ---------- | ------------------------------ |
| food               | string     | null: false                    |
| date               | date       | null: false                    |
| meal_time          | integer    | null: false                    |

### Association
- belongs_to :baby



