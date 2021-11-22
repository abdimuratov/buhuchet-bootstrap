<template>
  <!-- Задача №1 для frontend-разработчика (верстка):
Необходимо сверстать макет, в качестве основы использовать css-framework Bootstrap
 +1 В шапке сайта изображение располагается по центру и заполняет весь блок
 ?2 Контакт страницы может быть от 1 до 1000 строк
 +3 Меню располагается в самом верху страницы:
  +◦ Слева пункты перехода по разделам сайта (с подменю при необходимости)
  +◦ Справа пункты входа регистрации
 +4 Количество пунктов подменю может быть от 1 до 10
 +5 Эффект для разворачивания подменю выбираете самостоятельно
 +6 Вернее меню является фиксированным и не должно скрываться при прокрутке страницы
 -7 Подвал реализуется на усмотрение
 +8 При верстке необходимо учитывать различные экраны (desktop, mobile) -->

  <b-navbar toggleable="md" type="dark" variant="primary" sticky="true">
    <b-container fluid="xl">
      <b-navbar-brand to="/">Учёт.Бухгалтерия</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item to="/todo">Задачи</b-nav-item>
          <b-nav-item-dropdown left>
            <template #button-content>
              <em>Категории</em>
            </template>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
            <b-dropdown-item href="#">Шапки</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em>User</em>
            </template>
            <b-dropdown-item to="/profile">Профиль</b-dropdown-item>
            <b-dropdown-item to="/">Выйти</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-container>
  </b-navbar>
</template>

<style>
.navbar {
  background-image: url("https://images.unsplash.com/photo-1637507143792-66d72198f87e?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80");
  background-position: center;
  background-size: cover;
}
</style>
