# README

## usersテーブル

| Column             | Type   | Options                   |
| ------------------ | ------ | ------------------------- |
| email              | string | null: false, unique: true |
| ncrypted_password  | string | null: false               |
| name               | string | null: false               |
| profile            | text   | null: false               |
| occupation         | text   | null: false               |
| name               | text   | null: false               |

## prototypesテーブル

| Column             | Type      | Options                        |
| ------------------ | ----------| ------------------------------ |
| title              | string    | null: false                    |
| catch_copy         | text      | null: false                    |
| concept            | text      | null: false                    |
| user               | reference | null: false, foreign_key: true |

## commentsテーブル

| Column             | Type      | Options                        |
| ------------------ | ----------| ------------------------------ |
| content            | text      | null: false                    |
| prototype          | reference | null: false, foreign_key: true |
| user               | reference | null: false, foreign_key: true |