Скрипт создания БД и ее наполнения информацией находbтся в resources/database и исполняtтся автоматически при деплое
проекта в томкате. Если по какой то причине выдаст ошибку обращения к базе данных (у меня такое было при обратном
разворачивании проекта с GitHub то надо закомментить в mvc-dispetcher-servlet.xml следующие строки
 <!--<jdbc:initialize-database data-source="dataSource">
        <jdbc:script location="classpath:initDB.sql"/>
     </jdbc:initialize-database> -->