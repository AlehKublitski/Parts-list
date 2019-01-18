Скрипт создания БД и ее наполнения информацией находится в папке /resources/ и исполняется автоматически при деплое
проекта в томкате. Если по какой то причине выдаст ошибку обращения к базе данных (у меня такое бывало при обратном
разворачивании проекта с GitHub то надо закомментить в mvc-dispetcher-servlet.xml следующие строки
 <!--<jdbc:initialize-database data-source="dataSource">
        <jdbc:script location="classpath:initDB.sql"/>
     </jdbc:initialize-database> --> 
     
     и скрипт запустить отдельно
