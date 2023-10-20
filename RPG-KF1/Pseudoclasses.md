[[CompSci/Pseudoclasses]] pour [[RPG-KF1]]

# Pickable pseudoclass

```cpp
class Pickable : public Godot::Node3D {
	private:
		std::string  itemName;
		std::string  description;
		Godot::Scene inventoryScene;
		bool         consumeOnUse;

	public:
		Pickable(std::string itemName="dumy item", std::string description="dummy item description", Godot::Scene inventory_scene=BASIC_INVENTORY_ITEM_SCENE, bool consumeOnUse=false);
		
		virtual void use(Entity user);
		virtual void pickup(Entity user);
		virtual void drop(Entity user);
}
```

## Weapon pseudoclass

```cpp
class Weapon : public Pickable {
	private:
		double       baseDamages;
		Godot::Scene inHandScene
	
	public:
		Weapon(std::string itemName="dummy weapon", std::string description="dummy weapon description", Godot::Scene inventoryScene=BASIC_INVENTORY_WEAPON_SCENE, bool consumeOnUse=false, double base_damages=1.0, Godot::Scene inHandScene=BASIC_WEAPON_SCENE);
		
		void use(Entity user) override;
		void pickup(Entity user) override;
		void drop(Entity user) override;
		
		void gets_unequipped(Entity user);
		void gets_equipped(Entity user);
	
	private:
		virtual float get_damages(Entity user) = 0;
		virtual bool is_hitting(Entity user, Entity target);
}
```

### Sword pseudoclass

```cpp
class Sword: public Weapon {
	private:
		double reachDistance;
		double reachAngle;
	
	public:
		Sword(std::string itemName="dummy sword", std::string description="dummy sword description", Godot::Scene inventoryScene=BASIC_INVENTORY_SWORD_SCENE, bool consumeOnUse=false, double reachDistance=1.0, double reachAngle=45.0, double base_damages=1.0, Godot::Scene inHandScene=BASIC_SWORD__SCENE)
	
	private:
		float get_damages(Entity user) override;
		bool is_hitting(Entity user, Entity target) override;
}
```

# Entity pseudoclass

```cpp
class Entity : public Godot::Node3D {
	private:
		std::string                     entityName;
		Godot::Scene                    entityScene;
		double                          hp;
		std::map<std::string, Pickable> inventory;
		int                             baseInventorySize;
	
	public:
		Entity(std::string entityName="dummy entity", Godot::Scene entityScene=BASIC_ENTITY_SCENE, double hp=100.0, std::map<std::string, Pickable> inventory={});
		
		virtual bool should_die();
		virtual void be_attacked(double damages);
		
		void die();
}
```

## Player pseudoclass

```cpp
class Player : public Entity {
	private:
	    double pickupReach
		Weapon equippedLeftHand;
		Weapon equippedRightHand;
		Armor  equippedArmor;
	
	public:
		Player(std::string entityName="dummy player", Godot::Scene entityScene=BASIC_PLAYER_SCENE, double hp=100.0, std::map<std::string, Pickable> inventory={}, double pickupReach=2.0, Weapon equippedLeftHand=BASIC_HAND_EQUIPMENT, Weapon equippedRightHand=BASIC_HAND_EQUIPMENT, Armor equippedArmor=BASIC_ARMOR);
		
		void use_left();
		void use_right();
		
		void unequip_left();
		void unequip_right();
		
		void equip_left(Weapon newWeapon);
		void equip_right(Weapon newWeapon);
		
		void drop_left();
		void drop_right();
		
		void drop_weapons();
		void drop_all();
		
		void be_attacked(double damages) override;
		
		void grab_nearest(std::vector<Pickable> pickables);
}
```
