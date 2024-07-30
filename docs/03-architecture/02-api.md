# API

## Описание сущности User (Пользователь)

1. User
    - Nickname (String)
    - Email (String)

## Функции (эндпониты)

1. CRUDS (create, read, update, delete, search) для пользователей (User)

## Описание сущности Competition (Конкурс)

1. Competition:
    - UUID (String)
    - Title (String)
    - Avatar (Byte[])
    - Rules (Byte[])
    - DateStart (DateTime)
    - Stages (Stage[])
    - Judges (User [])
    - Moderators (User[])

## Функции (эндпониты)

1. CRUDS (create, read, update, delete, search) для конкурсов (Competition)

## Описание сущности Stage (Этап)

1. Stage
    - UUID (String)
    - Title (String)
    - Status (StageStatus)
    - Type (StageType)
    - Players (User[])
    - Judges (User[])
    - CompetitionUUID (UUID)
    - DateStart (DateTime)
    - DateEnd (DateTime)
    - WinnersCount (Integer)

## Функции (эндпониты)

1. CRUDS (create, read, update, delete, search) для конкурсов (Competition)

## Описание сущности StageType (Справочник - тип этапа)

1. StageType (enum)
    - QUALIFYING
    - PLAY_OFF

## Функции (эндпониты)

1. read

## Описание сущности StageStatus (Справочник - статус этапа)

1. StageStatus (enum)
    - WAITING
    - ACTIVE
    - GRADING
    - FINISHED

## Функции (эндпониты)

1. read

## Описание сущности Track (Работа для конкурса)

1. Track
   - Title
   - mp3 (Byte[])
   - txt (Byte[])
   - PlayerUUID (UUID)
   - StageUUID (UUID)
   - Grades (Grade [])

2. Track
   - Title (String)
   - UserNickName (String)
   - mp3Link (String)
   - txtLink (String)
   - Grades (Grade [])
## Функции (эндпониты)

1. POST /api/track/add
2. GET /api/track/get/{StageUUID}/{PlayerUUID}

## Описание сущности Grade (Оценка работы)

1. Grade
   - Value (Boolean)
   - Judge (User)
   - StageUUID (String)
   - UserNickname (String)

## Функции (эндпониты)

1. CRUDS (create, read, update, delete, search) для работ для конкурса (Track)

## Описание сущности Pair (Пары этапа play-off)

1. Pair
   - UserNickName1 (String)
   - UserNickName2 (String)
   - StageUUID (String)

## Функции (эндпониты)
1. CRUDS (create, read, update, delete, search) для работ для конкурса (Track)

